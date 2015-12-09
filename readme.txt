◎ Visual Studio
https://www.visualstudio.com/zh-tw/products/visual-studio-community-vs.aspx

微軟Visual Studio軟體編輯器，於2010後開放為免費開發平台。
其主要以開發.NET Framework為主的PC、Web軟體，諸如Windows Software、ASP.NET、Web Service等。

然而直到2013、2015等版本，更加擴大為可用於開發多語言、網頁平台程式，亦提供開發者轉移對不同平台與環境的開發，諸如可開發用於Windows Phones、Android、iOS等平台的應用程式。

◎ Visual Studio Tools for Apache Cordova
https://www.visualstudio.com/features/cordova-vs
http://cordova.apache.org/docs/en/latest/guide/overview/

V.S軟體開發環境是使用Apache Cordova為核心驅動其轉換於各種平台的運行，其主要使用語言為HTML、CSS、JS。
Appache Cordova是一套開放式行動裝置開發框架，他提供標準的網頁技術，諸如HTML5、CSS3、JavaScript等規範，並用於跨平台開發，避免使用個行動裝置平台的原生開發語言(Native Development Language)。

Apache Cordova規範於2012年10月，為Apache Software Foundation(ASF)的最高級計畫。

Apache Cordova使用原則：
- 行動裝置開發者且期望擴大應用程式可含括平台，但不希望依平台語言與工具重做(re-implement)。
- 行動裝置開發者且希望發佈網頁應用程式，使其封裝可分佈於各種應用程式商店。
- 行動裝置開發者有興趣混合原生應用程式單元和WebView(特殊瀏覽器視窗)，使其可存取裝置API，或開發Plugin介面介於Native與WebView單元。

在Visual Studio環境下使用Apache Cordova
https://msdn.microsoft.com/zh-tw/library/dn771545.aspx

◎ PhoneGap 與 Cordova 的實際差異
http://blog.tiger-workshop.com/difference-between-phonegap-and-cordova/
http://phonegap.com/2012/03/19/phonegap-cordova-and-what%E2%80%99s-in-a-name/

按照官方的說法 PhoneGap 是 Cordova 的一個 distribution。
PhoneGap is a distribution of Apache Cordova. 
You can think of Apache Cordova as the engine that powers PhoneGap, similar to how WebKit is the engine that powers Chrome or Safari.

◎ Phonegap與Titanium
http://www.developereconomics.com/pros-cons-top-5-cross-platform-tools/
http://www.xcubelabs.com/our-blog/phonegap-vs-titanium-comparison/

Phonegap：
Control on app release: 

If you want absolute control on the app release and bypass the review processes of the platform specific app stores, pick PhoneGap. Since PhoneGap apps are more like app enclosed websites, you can release/update websites as frequently as you would want to and the app is instantly updated for all of your users.

如果你期望對應用程式的絕對版本控制權，且審略各平台的審核問題，選擇PhoneGap。
PhoneGap本身為封裝網頁的應用程式，你可以透過release、update網頁來達到版本控制。

Porting an existing web app to mobile: 

If you have the business logic built and the website already working, then PhoneGap route is the quickest, provided you can quickly make most of your web pages / website mobile friendly.

若你的商業邏輯已經建置於網站端，使用PhoneGap可較為快速轉移。

Support all major mobile platforms: 

PhoneGap is the choice here, it supports iOS, Android, Blackberry 10, Windows 8 and Windows Phone 8, Amazon Fire OS and Tizen. Since the framework and the architecture of PhoneGap are simple, they can be quickly ported to any new platform that may be announced in the future. Titanium, on the other hand, currently supports iOS, Android with BB 10 and Windows (recently added). Adding a new platform to the list supported by Titanium takes a lot of effort and Titanium may or may not choose to support it.

PhoneGap可提供的平台包括，iOS、Android、Blackberry 10、Windows 8、Windows Phone 8、Amazon Fire OS、Tizen。
PhoneGap由於其框架與架構簡單，使其可以快速移植於各種平台；Titanium，目前提供iOS、Android、Blackberry 10、Windows，查詢目前可支援的平台需花費功夫查詢，且可能沒有支援。

Software and Hardware needed (infra): 

PhoneGap applications can be built on any system with just a browser. But tools like Dreamweaver, etc., can be used to help in the process. You would need to have the platform specific OS, SDK, and IDEs only if you want to build the application for deployment on your own machine. You can use a service called PhoneGap Build to build your apps for all supported platforms on the cloud and get the binaries. Titanium, on the other hand, requires platform specific hardware/software/SDKs to be installed to develop and build the apps.

PhoneGap應用程式可建置於各種系統，只需擁有瀏覽器，諸如，Dreamweaver等，皆可在開發過程中派上用場。
你只需要該平台作業系統、開發工具、編輯器即可對選定的裝置開發。
Titanium，需要安裝指定平台的硬體、軟體、SDK。

Programming Languages and Technologies: 

Although Titanium uses Javascript, XML, etc., to create the apps, the development team must understand the terminology and the constructs of the native applications to build the UI of the apps. PhoneGap does not need this. As long as you are good with HTML/CSS and Javascript you can go ahead and build the UI using any JS framework you like (JQuery Mobile).

Titanium使用JavaScript、XML等，開發團隊仍需了解其語法與建構原生元件的關聯。
PhoneGap使用HTML、CSS、JavaScript，你可使用JS框架工具直接建立UI。

Titanium：
http://www.appcelerator.com/product/

Need native UI, but do not know platform specific languages: 

Titanium wins, because your app can be deployed to all platform specific stores that are currently supported by Titanium. With PhoneGap, your app UI will not be native and performance will depend on the web browser of the platform and its limitations.

Titanium語法即可對其提供的原生元件進行操作，若使用PhoneGap，UI將不會是原生且效能將依賴網頁瀏覽器，且各平台的限制不同。


=========================

Reference : https://appery.io/appbuilder/

