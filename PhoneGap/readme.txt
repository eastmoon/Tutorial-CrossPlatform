Office web-site�G
http://phonegap.com/

�� Install Phonegap�G

�x��зǵ{��
http://phonegap.com/install/

1. Install NodeJS
Titanium�w�˳n��|�]�A�w��NodeJS�A�[��e�i�H�`�N��Titanium�w�ˤ覡�ۦ���Phonegap�C
�Y�����L�w��NodeJS�A�i�ܨ�x�����(https://nodejs.org/en/)�U���C

2. Open command line and execute�ynpm install -g phonegap�z
�ϥΩR�O�C�A�ð���ynpm install -g phonegap�z�A�z�LNodeJS�U��phonegap

3. �إ߱M�רóz�L�����������դu�����示�e�C
�ثe�@���T�ؤ覡�i����աG
(1 ADV 
http://docs.phonegap.com/en/edge/guide_cli_index.md.html#The%20Command-Line%20Interface_test_the_app_on_an_emulator_or_device

�ϥΦ�ʸ˸m�������A�ѦҤW��ާ@�C
�ycordova emulate android�z�A�ŧi�ó]�mAndroid�������ҡF���ѩ��l���ҳ]�m�ӮɡA�O�_�i���T���椴�����ҡC
�ycordova run android�z�A�N�M�װ����Android�������ҡF�`�N�A���ҰʩR�O�Ҧ��A�N���|���m�����檺�M�צ�m�A�~�i���T����C

(2 Phonegap desktop
http://docs.phonegap.com/getting-started/1-install-phonegap/desktop/

Phonegap desktop�O�@�M²���}�o���դu��A�e��ݦw�˨�˳n��
- PhoneGap Desktop�A�w�˩�sĶ�Ϊ����x�F���n�鴣�ѫظm�M�׻P�ҰʱM�״��ժA�Ⱦ��C
- PhoneGap Developer App�A�w�˩�n���ժ����x�A���n�鬰�K�O�C

�o�M����O�z�LDesktop�Ұʤ@��Web Service�A�å�App�g�L�ϰ�����s�u�ܪA�ȫ���J�M�רð����ؼи˸m�C
�ѩ�Desktop�ȬO���ѫظm�M�סB�ҰʪA�ȳo�ⶵ�D�n�\��A���s�褴���ϥκ����s��u��A�p�GDreamwave�C

�� Desktop�n�饻���O�@�M��U�u��A�Y�L�k�T�w����O�_���`�A�i�H�z�L�U�夺�e����A�ȡA���˾\�䷾�q���e�C
http://phonegap.com/blog/2014/04/23/phonegap-developer-app/

�YApp�L�k�s���θ��J�M�סA�T�{�U�z���D�O�_����ѨM�G

1. disable firewall and AV software on your computer
2. make sure your router/network doesn't have a hardware firewall, if it does either disable it or configure it to allow traffic on the port that PhoneGap Desktop is using to serve (usually this is on a corporate network and you won't have the ability to change the config, if that's the case use a non-corporate network)
3. make sure that both your computer and mobile device are connected to the same network
4. make sure that you are using the latest versions of PhoneGap Desktop and the PhoneGap Developer apps

(3 Build
http://docs.phonegap.com/en/edge/guide_cli_index.md.html#The%20Command-Line%20Interface_build_the_app

�Y�W�z�覡�]�}�o���ҵ��Ѧh����ɭP�]�m�����A�i�H�ĥΫظm(Build)�M�ת��覡�A������X�w��(�ʸ�)�n�鵹�ؼи˸m�A�z�L�w�˨ӥ��T����n��C
�ycordova platforms ls�z�A�ˬd��e���ҥi�ظm���M�������A��Y���Ҥ��s���n��}�o�M��(SDK�ASoftware Developer Kit)
�ycordova platform add XXX�z�A�YXXX���s�b���Ҥ��A�N��[�J�F�禳remove���O�N��R���C
�ycordova build XXX�z�A�N�M�׫ظm���i�bXXX���Ҥ����檺�w�˵{���F��X���ɮ׷|�b�M�ק���platforms/XXX�U�A�ԲӦ�m�i�˾\�sĶ���G�C


�� PhoneGap �ɮ׵��c
http://docs.phonegap.com/develop/hello-world-explained/

PhoneGap�O�@�MApache cordova�������M��A�]���A�b�D���c�W�i�H�Ѧ�Apache cordova�������ɮ׻����C
Apache Cordova�]�w�ɻ����Ahttps://cordova.apache.org/docs/en/latest/config_ref/index.html
�L�nAngular for Cordova�d���ɮסAhttps://github.com/Microsoft/cordova-samples

�z�LPhoneGap�إߪ��ɮר�[�c�p�U�G
�� platforms
�|andorid
�|ios

���M�׳]�m���������xSDK�P������X�C

�� plugins

���M�׳]�w�ϥΪ��~���u��A�Ѧp�q�����A��T���C
�ѩ�Cordova��h�W��w�������ܬ������D�n�ާ@�A����L��ʸ˸m���ҫh�HPlugin�覡���J���u��A�A�g��JavaScript�I�s�C

��e�B�~�X�R���~���u��C��p�U��G
http://docs.phonegap.com/plugin-apis/

�� www
�|css
�|img
�|js
�|res
�|spec
   �|lib

www����������ɮסA���F�D�n�ɮ׻����p�U��
http://docs.phonegap.com/develop/hello-world-explained/

��h�W�S�S�O�W�w���]�m�M�ɮק�����ϥΡA�ѦҷL�n���ɮ׽d�ҥ�i�C
�Y�H�зǴ��Ѩӵ����A�䵲�c�W�d���G
css�A�˦��]�w�ɮ�
img�A�v���ɮ�
js�A�M�׾ާ@��JavaScript�ɮ�
res�A�M�׸귽�ɮסA�ϥ��ɵ��A�Ω����γ~���v����
spec�A�M��JavaScript��Ʈw�ɮסA�ҦpAngularJS�Bjasmine��

�� PhoneGap plug-in

Hello world sample
https://github.com/don/cordova-plugin-hello

Android plugins
https://cordova.apache.org/docs/en/dev/guide/platforms/android/plugin.html

iOS plugins
https://cordova.apache.org/docs/en/dev/guide/platforms/ios/plugin.html

�� Build error issue

---- Issue ----
Cordova : [Error: Please install Android target: ��android-21��
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