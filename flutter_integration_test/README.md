# flutter_integration_test

A Flutter integration test example.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://flutter.dev/docs/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://flutter.dev/docs/cookbook)
- [Testing: Integration testing](https://flutter.dev/docs/testing/integration-tests)
- [Package: integration_test](https://pub.dev/packages/integration_test)

For help getting started with Flutter, view our
[online documentation](https://flutter.dev/docs), which offers tutorials,
samples, guidance on mobile development, and a full API reference.

## Usage

### for Android emulator
- Launch the Android emulator
  - Launch from Android Studio
    1. Click menu [Tools -> AVD Manager]
    1. Click any ｌLaunch emulator action icon
  - Launch from Shell

ex) for windows on Command Prompt
```
> cd C:\Users\{UserName}\AppData\Local\Android\sdk\emulator
> emulator -list-avds
Pixel_3_API_28
> emulator @Pixel_3_API_28
```

- Run integration tests
```
> git clone https://github.com/itsnowcode/flutter-example.git
> cd flutter-example
> cd flutter_integration_test
> flutter drive --driver=test_driver/integration_test.dart --target=integration_test/counter_test.dart
```

### for Web 

- Run WebDriver

ex) ChromeDriver
```
chromedriver --port=4444
```
[Download ChromeDriver](https://chromedriver.chromium.org/downloads)

> ChromeDriver uses the same version number scheme as Chrome.

- Run integration tests
```
flutter drive --driver=test_driver/integration_test.dart --target=integration_test/counter_test.dart -d web-server
```