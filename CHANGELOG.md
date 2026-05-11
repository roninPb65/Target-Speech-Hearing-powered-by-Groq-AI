# Changelog

All notable changes to the TGH - Target Speech Hearing project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2026-05-10

### Added
- Initial release of TGH - Target Speech Hearing
- Real-time audio recording from browser microphone
- Integration with Groq AI API for speech transcription
- Support for multiple Whisper model variants:
  - whisper-large-v3 (Best Quality)
  - whisper-large-v3-turbo (Faster)
  - distil-whisper-large-v3-en (English Only - Fast)
- Live audio visualization with animated bars
- Timestamped transcription output
- Session-based transcription history
- Local storage for API key persistence
- Responsive design for mobile and desktop
- Error handling and user feedback
- Browser compatibility checks
- MIT License

### Features
- 🎙️ One-click recording with visual feedback
- ⚡ Lightning-fast transcription via Groq AI
- 📊 Real-time audio level visualization
- 💾 Automatic API key storage
- 📝 Accumulative transcription history
- 🔐 Secure client-side processing
- 📱 Mobile-responsive interface

### Technical Details
- Pure vanilla JavaScript (no frameworks required)
- Web Audio API for audio processing
- MediaRecorder API for audio capture
- Groq AI Whisper API integration
- Local Storage API for persistence
- CSS3 animations and gradients

---

## [Unreleased]

### Planned Features
- Language selection for multilingual support
- Export transcriptions (TXT, JSON, SRT formats)
- Speaker diarization
- Real-time streaming transcription
- Audio file upload support
- Translation capabilities
- Custom vocabulary/terminology
- Keyboard shortcuts
- Dark mode theme
- Transcription editing
- Search within transcriptions
- Copy to clipboard button
- Download audio recordings
- Confidence scores display

---

[1.0.0]: https://github.com/your-username/tgh-speech-hearing/releases/tag/v1.0.0
