
# 🎤 Voice Message Package

The `voice_message_package` is a Flutter plugin that allows developers to easily add voice message functionality into their apps. It provides recording, playback, and visualization of audio messages.

## 🚀 Features

- Record voice messages
- Playback with waveform
- Visual indicators for sent/received status
- Customizable UI

## 🛠️ Installation

Add the following to your `pubspec.yaml`:

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

## 🧱 Usage

```dart
VoiceMessage(
  audioSrc: 'https://example.com/audio.mp3',
  played: false,
  me: true,
  onPlay: () {
    // your logic here
  },
)
```

## 📝 License

MIT © [sorydima](https://github.com/sorydima)
