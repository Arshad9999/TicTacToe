# Tic-Tac-Toe Android App

A two-player Tic-Tac-Toe game built as a native Android application with Java and XML layouts. Players enter their names, take turns on a 3×3 board, and see the match result in the app.

> [!NOTE]
> This is an Android project, not a command-line Java program. It requires the Android SDK and must be built with Gradle or Android Studio.

## Project status

- **Platform:** Android
- **Language:** Java
- **Minimum Android version:** API 21 (Android 5.0)
- **Compile and target SDK:** API 32
- **Build system:** Gradle 7.2 with Android Gradle Plugin 7.1.1
- **Recommended JDK:** 11

## Prerequisites

Install one of the following:

1. Android Studio with Android SDK Platform 32 and Build Tools installed; or
2. JDK 11 plus the Android command-line tools, with `ANDROID_HOME` or `ANDROID_SDK_ROOT` pointing to the SDK.

The checked-in Gradle wrapper downloads the required Gradle distribution automatically.

## Setup

```bash
git clone https://github.com/Arshad9999/TicTacToe.git
cd TicTacToe
chmod +x gradlew
```

Open the directory in Android Studio and allow Gradle synchronization to finish. Select an emulator or connected Android device and run the `app` configuration.

## Command-line validation

With Android SDK Platform 32 available:

```bash
./gradlew testDebugUnitTest
./gradlew assembleDebug
```

The debug APK is generated under `app/build/outputs/apk/debug/`.

Instrumented tests require a running emulator or connected device:

```bash
./gradlew connectedDebugAndroidTest
```

GitHub Actions runs the local unit-test task and assembles the debug APK for every pull request and push to the default branch.

## Project structure

```text
app/src/main/java/       Activities and game behavior
app/src/main/res/layout/ Android XML layouts
app/src/main/res/drawable/ Game images and visual assets
app/src/test/            Local JVM unit tests
app/src/androidTest/     Device or emulator tests
```

## Fork and contribution provenance

This repository is a fork of [Mohd-Farhan/TicTacToe](https://github.com/Mohd-Farhan/TicTacToe). See [FORK_NOTES.md](FORK_NOTES.md) for the audited attribution and contribution notes. Upstream authors retain credit for their work; do not present the full project as independently authored.

## License

The project retains its existing [Apache License 2.0](LICENSE.md). Preserve upstream copyright and attribution notices when redistributing it.
