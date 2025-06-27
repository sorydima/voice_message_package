
# 📦 Voice Message Package Wiki

Welcome to the official Wiki for the **Voice Message Package**, a Flutter-based audio messaging component. This package provides easy-to-use tools for recording, sending, receiving, and playing back voice messages within your Flutter apps.

---

## 📌 Overview

**voice_message_package** enables seamless integration of voice messaging functionality. It simplifies:

- Recording voice messages
- Displaying voice message UI
- Playback with waveform or visual cues
- Integration with chat systems

---

## 🚀 Getting Started

### 1. Installation

Add the package to your `pubspec.yaml`:

```yaml
dependencies:
  voice_message_package:
    git:
      url: https://github.com/sorydima/voice_message_package.git
```

Then run:

```bash
flutter pub get
```

---

### 2. Permissions

Make sure you request and configure the following permissions:

**Android** (`android/app/src/main/AndroidManifest.xml`):

```xml
<uses-permission android:name="android.permission.RECORD_AUDIO"/>
<uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE"/>
```

**iOS** (`ios/Runner/Info.plist`):

```xml
<key>NSMicrophoneUsageDescription</key>
<string>We need access to your microphone to record voice messages.</string>
```

---

## 🧱 Basic Usage

```dart
import 'package:voice_message_package/voice_message_package.dart';

VoiceMessage(
  audioSrc: 'https://example.com/audio.mp3',
  played: false,
  me: true,
  onPlay: () {
    // handle play logic
  },
)
```

You can also configure UI parameters such as `me`, `played`, `duration`, and `onPlay`.

---

## 🎛️ Features

- 🎙️ Voice recording
- ⏯️ Play/pause control
- 📊 Waveform visualization (optional)
- 🎨 Customizable bubble appearance
- 📤 Upload logic support

---

## 🛠️ Customization

You can customize:

- Colors for sent/received messages
- Icons for play/pause
- Duration format
- Callback hooks on play/pause events

Example:

```dart
VoiceMessage(
  audioSrc: '...',
  me: false,
  played: true,
  onPlay: () => print("Audio played"),
  meBgColor: Colors.blue,
  contactBgColor: Colors.grey,
)
```

---

## 🧪 Testing

To test recording functionality, use an emulator or real device with microphone access.

---

## 📂 Folder Structure

```bash
voice_message_package/
├── lib/
│   ├── voice_message.dart       # Main widget
│   └── ...                      # Additional components/utilities
├── example/                     # Example usage
├── README.md
└── pubspec.yaml
```

---

## 🧩 Integration Tips

- Pair with chat packages (e.g., `flutter_chat_ui`)
- Combine with cloud storage for saving messages
- Use local caching for smoother UX

---

## 🧑‍💻 Contributors

Maintained by [sorydima](https://github.com/sorydima). Contributions welcome! Feel free to open issues or PRs.

---

## 📜 License

This project is licensed under the MIT License.
