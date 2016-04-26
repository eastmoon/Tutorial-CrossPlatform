Office web-site：
http://phonegap.com/

◎ Install Phonegap：

官方標準程序
http://phonegap.com/install/

1. Install NodeJS
Titanium安裝軟體會包括安裝NodeJS，觀察內容可以注意到Titanium安裝方式相似於Phonegap。
若本身無安裝NodeJS，可至其官方網站(https://nodejs.org/en/)下載。

2. Open command line and execute『npm install -g phonegap』
使用命令列，並執行『npm install -g phonegap』，透過NodeJS下載phonegap

3. 建立專案並透過虛擬機等測試工具檢驗內容。
目前共有三種方式進行測試：
(1 ADV 
http://docs.phonegap.com/en/edge/guide_cli_index.md.html#The%20Command-Line%20Interface_test_the_app_on_an_emulator_or_device

使用行動裝置模擬器，參考上文操作。
『cordova emulate android』，宣告並設置Android模擬環境；但由於初始環境設置耗時，是否可正確執行仍需驗證。
『cordova run android』，將專案執行於Android模擬環境；注意，先啟動命令模式，將路徑移置欲執行的專案位置，才可正確執行。

(2 Phonegap desktop
http://docs.phonegap.com/getting-started/1-install-phonegap/desktop/

Phonegap desktop是一套簡易開發測試工具，前後需安裝兩樣軟體
- PhoneGap Desktop，安裝於編譯用的平台；此軟體提供建置專案與啟動專案測試服務器。
- PhoneGap Developer App，安裝於要測試的機台，此軟體為免費。

這套機制是透過Desktop啟動一個Web Service，並由App經過區域網路連線至服務後載入專案並執行於目標裝置。
由於Desktop僅是提供建置專案、啟動服務這兩項主要功能，對於編輯仍須使用網頁編輯工具，如：Dreamwave。

※ Desktop軟體本身是一套協助工具，若無法確定執行是否正常，可以透過下文內容執行服務，並檢閱其溝通內容。
http://phonegap.com/blog/2014/04/23/phonegap-developer-app/

若App無法連結或載入專案，確認下述問題是否能夠解決：

1. disable firewall and AV software on your computer
2. make sure your router/network doesn't have a hardware firewall, if it does either disable it or configure it to allow traffic on the port that PhoneGap Desktop is using to serve (usually this is on a corporate network and you won't have the ability to change the config, if that's the case use a non-corporate network)
3. make sure that both your computer and mobile device are connected to the same network
4. make sure that you are using the latest versions of PhoneGap Desktop and the PhoneGap Developer apps

(3 Build
http://docs.phonegap.com/en/edge/guide_cli_index.md.html#The%20Command-Line%20Interface_build_the_app

若上述方式因開發環境等諸多限制導致設置不順，可以採用建置(Build)專案的方式，直接輸出安裝(封裝)軟體給目標裝置，透過安裝來正確執行軟體。
『cordova platforms ls』，檢查當前環境可建置的專案類型，亦即環境內存有軟體開發套件(SDK，Software Developer Kit)
『cordova platform add XXX』，若XXX不存在環境內，將其加入；亦有remove指令將其刪除。
『cordova build XXX』，將專案建置成可在XXX環境內執行的安裝程式；輸出的檔案會在專案夾內platforms/XXX下，詳細位置可檢閱編譯結果。


◎ PhoneGap 檔案結構
http://docs.phonegap.com/develop/hello-world-explained/

PhoneGap是一套Apache cordova的延伸套件，因此，在主結構上可以參考Apache cordova的相關檔案說明。
Apache Cordova設定檔說明，https://cordova.apache.org/docs/en/latest/config_ref/index.html
微軟Angular for Cordova範例檔案，https://github.com/Microsoft/cordova-samples

透過PhoneGap建立的檔案其架構如下：
○ platforms
└andorid
└ios

本專案設置的對應平台SDK與相關輸出。

● plugins

本專案設定使用的外部工具，諸如電池狀態資訊等。
由於Cordova原則上制定對網站顯示相關的主要操作，對於其他行動裝置環境則以Plugin方式載入為工具，再經由JavaScript呼叫。

當前額外擴充的外部工具列表如下文：
http://docs.phonegap.com/plugin-apis/

○ www
└css
└img
└js
└res
└spec
   └lib

www為網頁實際檔案，除了主要檔案說明如下文
http://docs.phonegap.com/develop/hello-world-explained/

原則上沒特別規定應設置和檔案夾為何使用，參考微軟的檔案範例亦可。
若以標準提供來評估，其結構規範為：
css，樣式設定檔案
img，影像檔案
js，專案操作用JavaScript檔案
res，專案資源檔案，圖示檔等，用於手機用途的影像檔
spec，專案JavaScript函數庫檔案，例如AngularJS、jasmine等

◎ PhoneGap plug-in

Hello world sample
https://github.com/don/cordova-plugin-hello

Android plugins
https://cordova.apache.org/docs/en/dev/guide/platforms/android/plugin.html

iOS plugins
https://cordova.apache.org/docs/en/dev/guide/platforms/ios/plugin.html

◎ Build error issue

---- Issue ----
Cordova : [Error: Please install Android target: “android-21”
http://stackoverflow.com/questions/29396252/cordova-error-please-install-android-target-android-21

1. Goto modify project.properties, AndroidManifest.xml in
- myApp/platforms/android/
- myApp/platforms/android/CordovaLib/

2. Modify project.properties
# Project target.
target=[latest version]

3. AndroidManifest.xml
<uses-sdk android:minSdkVersion="14" android:targetSdkVersion="[lastest version]" />

4. lastest version look in 
---- Issue ----
C:\Program Files (x86)\Android\android-sdk\platforms