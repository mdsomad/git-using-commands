### Flutter Using Important Commands






- Flutter build app appbundle commant
```sh
flutter build appbundle
```



- Flutter clean commant
```sh
1. First Yah run kare
flutter clean
```



- Flutter clean commant
```sh
1. Yah 3 bhago Mein bat dega Example this is 1 --> app-armeabi-v7a-release.apk 
2. Yah 2 --> app-arm64-v8a-release.apk 
3. Yah 3 --> app-x86_64-release.apk
flutter build apk --split-per-abi
```



- Flutter Mein keystore File generate ka On Windows command
```sh
1. keystore File ka director add Karne Ka Tarika yah hai
2. Example This is -->  keytool -genkey -v -keystore C:\Users\mdsom\upload-keystore.jks -storetype JKS 3. -keyalg RSA -keysize 2048 -validity 10000 -alias upload

  keytool -genkey -v -keystore %userprofile%\upload-keystore.jks -storetype JKS -keyalg RSA -keysize 2048 -validity 10000 -alias upload
```




- Yah hai First Tarika SHA1 key Full details find command   or  recommended Tarika hai
```sh
1. First Tarika copy command paste VS Code Terminal then Enter
2. command setup Example yah hai --> keytool -list -v -keystore
3. "C:\Users\mdsom\.android\debug.keystore" -alias androiddebugkey -storepass android -keypass android

keytool -list -v -keystore "C:\Users\yourname\.android\debug.keystore" -alias androiddebugkey -storepass android -keypass android

```




- Yah hai Second Tarika SHA1 key Full details find command
```sh
1.  Second Tarika find SHA1 key first step location directory C:\Program Files\Java\jdk-18.0.1.1\bin & 2.  cmd then Enter Copy command paste then Enter

keytool -list -v -keystore %USERPROFILE%\.android\debug.keystore -alias androiddebugkey -storepass android -keypass android

```




- Flutter project application desktop ke liye enable
```sh
1. First command Run Terminal
flutter config --enable-linux-desktop
```



- Flutter project Create macos & linux model & Folder Create command VSCode Terminal
```sh
2.Second command Run Terminal
flutter create --platform=windows,macos,linux .

```
