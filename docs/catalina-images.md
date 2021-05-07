# Detail of what content each image

## mickjol/macos-catalina:base
- Catalina 10.15.7

## mickjol/macos-catalina:code
- macos-catalina:base
- Visual Studio Code 1.55.2
- Xcode 12.2

## mickjol/macos-catalina:cordova
- macos-catalina:code
- Homebrew 3.1.5
- NodeJs 14.16.1
- NPM 7.12.0
- Cordova 10.0.0 (telemetry off)

#### for build ios
- native-run 1.3.0
- xcode-select 2373
- ios-deploy 1.11.4
- cocoapods 1.10.1

#### for build android
- OpenJDK 8
- Android Studio 4.2
- Gradle 7.0