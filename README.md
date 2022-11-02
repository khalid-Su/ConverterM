<div align="center">

# Converter NOW

[<img src="https://img.shields.io/github/contributors/ferraridamiano/ConverterNOW?style=flat-square"
    alt="Contributors"
    height="30">](https://github.com/ferraridamiano/ConverterNOW/graphs/contributors)
[<img src="https://img.shields.io/static/v1?style=for-the-badge&message=PWA&color=5A0FC8&logo=PWA&logoColor=FFFFFF&label="
    alt="Open web app"
    height="30">](https://converter-now.web.app)
[<img src="https://img.shields.io/static/v1?style=for-the-badge&message=PayPal&color=00457C&logo=PayPal&logoColor=FFFFFF&label="
    alt="Donate paypal"
    height="30">](https://www.paypal.me/DemApps)

[<img src="https://img.shields.io/badge/maintained%20with-melos-f700ff.svg?style=flat-square"
    alt="Maintained with Melos">](https://github.com/invertase/melos)

<img src="fastlane/metadata/android/en-US/images/phoneScreenshots/1.jpeg" width="140"> <img src="fastlane/metadata/android/en-US/images/phoneScreenshots/2.jpeg" width="140"> <img src="fastlane/metadata/android/en-US/images/phoneScreenshots/3.jpeg" width="140"> <img src="fastlane/metadata/android/en-US/images/phoneScreenshots/4.jpeg" width="140"> <img src="fastlane/metadata/android/en-US/images/phoneScreenshots/5.jpeg" width="140">
</div>

## Why Converter NOW




[<img src="https://flathub.org/assets/badges/flathub-badge-en.png"
    alt="Download on Flathub"
    height="55">](https://flathub.org/apps/details/io.github.ferraridamiano.ConverterNOW)
[<img src="https://snapcraft.io/static/images/badges/en/snap-store-black.svg"
    alt="Get it from the Snap Store"
    height="55">](https://snapcraft.io/converternow)

### Windows

[<img src="https://getbadgecdn.azureedge.net/images/English_L.png"
    alt="Get it from the Microsoft Store"
    height="60">](https://www.microsoft.com/store/apps/9P0Q79HWJH72)

### Web
You can reach the PWA [here](https://converter-now.web.app).

## Build from source code
First you need to
[install flutter](https://docs.flutter.dev/get-started/install) and all the
tooling for your target platform (e.g. Android Studio for Android, etc.). Then
you have to activate a tool that is used to manage this repo, so you have to
type `dart pub global activate melos` to install it and `melos bootstrap` in the
root of the project in order to get all the dependencies and generate the
translations code. Then follow the instructions for the platform you target.

### Android
On Android you should first disable the signing option in
[`android/app/build.gradle`](https://github.com/ferraridamiano/ConverterNOW/blob/master/android/app/build.gradle#L70)
(just comment that line). Then you can type `flutter build apk --split-per-abi`
to compile the code. You can find the output in `build/app/outputs/flutter-apk`
folder.

### Linux
Type `flutter build linux` to build the Linux app. You can find the output in
`build/linux/x64/release/bundle`.

### Windows
Type `flutter build windows` to build the Windows app. You can find the output
in `build/windows/runner/Release`.

### Web
Type `flutter build web` to build the Web app. You can find the output in
`build/web`.

Note: if you deploy it not on the base path, add `--base-href=/path/` to the command above, change `/path/` with your path.

### iOS and MacOS
The app is not tested against iOS and MacOS, but you should be able to compile
it even for these platforms. You first need to generate the platform specific
code and then compile them.
