# BaghBondi Android Game

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white)
![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)
![Gradle](https://img.shields.io/badge/Gradle-02303A?style=for-the-badge&logo=gradle&logoColor=white)

An Android application built with Java using Android SDK 24. The game implements a rule-based opponent system where the tiger follows deterministic priority rules (capture > random move). Game state is managed through position arrays and SharedPreferences for persistent high score storage. UI uses custom drawable resources and ObjectAnimator for smooth piece movement animations. The board consists of 19 positions encoded as two-digit numbers (row+column) with special movement logic for center and corner positions.

## How to Run

1. **Prerequisites**: Android Studio or Android SDK with Gradle
2. **Build**: Run `./gradlew build` or open in Android Studio
3. **Install**: Connect Android device/emulator and run `./gradlew installDebug` or use Android Studio's Run button
4. **Requirements**: Android 4.1+ (API 16+)

## Game Rules

- **Player**: Controls 7 goats
- **Opponent**: Rule-based tiger
- **Objective**: Trap the tiger with no valid moves to win
- **Lose Condition**: If 3 or fewer goats remain

## How to Play

1. Tap a goat to select it
2. Tap a highlighted position to move
3. Tiger moves automatically after your turn
4. Score decreases by 100 per move

## Build

- Minimum SDK: 16
- Target SDK: 24
- Build with Android Studio or Gradle

## Features

- Rule-based tiger opponent
- Score tracking with high scores
- Smooth animations
- Win/lose screens

