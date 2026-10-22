# Snake Game (የእባብ ጨዋታ)

A modern, high-performance **Flutter** Snake Game with AdMob ads, rewarded revive system, customizable skins, invincibility shield power-ups, tactile haptic feedback, and multi-level difficulties.

---

## 📱 App Details
- **App Name:** `Snake Game`
- **Package Name:** `kaleb.snakegame.menen`
- **Framework:** Flutter (Dart) & Android
- **Language:** English

---

## 📂 Project Structure (Matching Standard Flutter Tree)
```
├── .dart_tool/
├── .idea/
├── android/
│   ├── app/
│   │   ├── src/main/
│   │   │   ├── AndroidManifest.xml (kaleb.snakegame.menen & AdMob App ID)
│   │   │   └── kotlin/kaleb/snakegame/menen/MainActivity.kt
│   │   └── build.gradle
│   ├── build.gradle
│   └── settings.gradle
├── build/
├── lib/
│   ├── main.dart
│   ├── models/
│   │   └── snake_models.dart
│   ├── services/
│   │   ├── ad_service.dart
│   │   └── vibration_service.dart
│   └── widgets/
│       ├── dialogs.dart
│       ├── dpad_controls.dart
│       ├── game_board.dart
│       └── game_hud.dart
├── test/
│   └── widget_test.dart
├── .gitignore
├── .metadata
├── analysis_options.yaml
├── snake_game.iml
├── pubspec.lock
├── pubspec.yaml
└── README.md
```

---

## 🎮 Key Features
1. **Initial Movement:** Starts moving downwards from top to bottom automatically.
2. **2-Life System & Rewarded Recovery:**
   - Players start with **2 Lives**.
   - Hitting a wall or tail uses 1 life with an invulnerability grace period.
   - When all lives are depleted, players can tap **"Continue Run (+3 Lives)"** to watch a rewarded ad and resume right where they left off with their score preserved. Rewards are granted only when the ad SDK confirms completion; closing or failing to load the ad grants no reward. **"Play Again"** also requires a completed rewarded ad.
3. **Controls:**
   - Ergonomic on-screen D-Pad (Up, Down, Left, Right).
   - Smooth swipe gestures directly on the game board.
4. **Food & Power-ups:**
   - Normal Red Apple (+10 pts).
   - Golden Star Bonus (+50 pts, 7-second countdown).
   - Invincibility Shield (6-second protection: wrap around walls and pass through own tail safely).
5. **Custom Snake Skins:**
   - Emerald Viper (Default)
   - Cyber Neon
   - Golden Dragon
   - Lava Serpent
   - Cosmic Amethyst
6. **Tactile Haptic Feedback:** Vibrations on eating, crashes, bonus pickup, and button taps.
7. **AdMob Integration:**
   - App ID: `ca-app-pub-7621875430117912~5112925480`
   - App Open: `ca-app-pub-7621875430117912/8018591749`
   - Persistent Banner: `ca-app-pub-7621875430117912/3608272128` (fixed at bottom with no close button)
   - Interstitial: `ca-app-pub-7621875430117912/1930947116`
   - Rewarded (2 Videos): `ca-app-pub-7621875430117912/8198428838`

---

## 🚀 How to Run in Flutter
```bash
flutter pub get
flutter run
```
