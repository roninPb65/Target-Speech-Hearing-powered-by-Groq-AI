# 🎯 TGH - Target Speech Hearing

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow.svg)
![Groq](https://img.shields.io/badge/Powered%20by-Groq%20AI-orange.svg)

A real-time speech-to-text application powered by Groq AI's ultra-fast Whisper models. Record audio directly from your browser and get instant, accurate transcriptions.

## ✨ Features

- 🎙️ **Real-time Audio Recording** - Record speech directly from your microphone
- ⚡ **Lightning-Fast Transcription** - Powered by Groq's industry-leading inference speed
- 📊 **Live Audio Visualization** - Visual feedback of audio levels as you speak
- 🔧 **Multiple Model Options** - Choose from different Whisper model variants
- 📝 **Timestamped Transcriptions** - Each recording is automatically timestamped
- 💾 **Session History** - All transcriptions accumulate in one session
- 🔐 **Secure API Key Storage** - Your API key is saved locally in your browser

## 🚀 Demo

[Live Demo](https://your-username.github.io/tgh-speech-hearing) _(Update with your GitHub Pages URL)_

## 📸 Screenshots

![TGH Interface](screenshots/tgh-interface.png)

## 🛠️ Technology Stack

- **Frontend**: Pure HTML5, CSS3, JavaScript (ES6+)
- **Audio Processing**: Web Audio API, MediaRecorder API
- **AI/ML**: Groq AI API (Whisper models)
- **Hosting**: GitHub Pages compatible (static site)

## 📋 Prerequisites

- Modern web browser with microphone support (Chrome, Firefox, Safari, Edge)
- Groq AI API key (free tier available)

## 🔧 Installation

### Option 1: Direct Download

1. Clone the repository:
```bash
git clone https://github.com/your-username/tgh-speech-hearing.git
cd tgh-speech-hearing
```

2. Open `tgh-speech-hearing.html` in your web browser

### Option 2: GitHub Pages

1. Fork this repository
2. Go to Settings → Pages
3. Select "main" branch as source
4. Your app will be available at `https://your-username.github.io/tgh-speech-hearing`

### Option 3: Local Server

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js
npx http-server
```

Then navigate to `http://localhost:8000/tgh-speech-hearing.html`

## 🔑 Getting Your Groq API Key

1. Visit [Groq Console](https://console.groq.com)
2. Sign up for a free account
3. Navigate to API Keys section
4. Create a new API key
5. Copy your API key (starts with `gsk_...`)

## 📖 Usage

1. **Enter API Key**
   - Paste your Groq API key in the input field
   - The key is automatically saved in your browser's local storage

2. **Select Model**
   - Choose from available Whisper models:
     - `whisper-large-v3` - Best quality
     - `whisper-large-v3-turbo` - Faster processing
     - `distil-whisper-large-v3-en` - English-only, fastest

3. **Start Recording**
   - Click "Start Recording" button
   - Grant microphone permissions if prompted
   - Speak clearly into your microphone
   - Watch the audio visualizer for feedback

4. **Stop & Transcribe**
   - Click "Stop" when finished speaking
   - Transcription appears automatically with timestamp

5. **Manage Transcriptions**
   - Multiple recordings accumulate in the session
   - Click "Clear" to reset all transcriptions

## 🎨 Customization

### Changing Colors

Edit the CSS variables in the `<style>` section:

```css
/* Primary gradient */
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);

/* Button colors */
.btn-record { background: #667eea; }
.btn-stop { background: #f59e0b; }
```

### Adjusting Audio Settings

Modify the audio constraints in the JavaScript:

```javascript
const stream = await navigator.mediaDevices.getUserMedia({ 
    audio: {
        echoCancellation: true,
        noiseSuppression: true,
        autoGainControl: true
    }
});
```

## 🌐 Browser Compatibility

| Browser | Support | Notes |
|---------|---------|-------|
| Chrome  | ✅ Full | Recommended |
| Firefox | ✅ Full | Recommended |
| Safari  | ✅ Full | Requires HTTPS or localhost |
| Edge    | ✅ Full | Chromium-based |
| Opera   | ✅ Full | Chromium-based |

**Note**: Microphone access requires HTTPS in production or localhost for development.

## 🔒 Privacy & Security

- ✅ All audio processing happens client-side
- ✅ Audio is sent directly to Groq API (not stored on any server)
- ✅ API keys are stored only in your browser's local storage
- ✅ No user data is collected or tracked
- ✅ No cookies or analytics

## 📊 Available Models

| Model | Speed | Quality | Language | Best For |
|-------|-------|---------|----------|----------|
| whisper-large-v3 | Medium | Highest | Multilingual | Accuracy-critical tasks |
| whisper-large-v3-turbo | Fast | High | Multilingual | General use |
| distil-whisper-large-v3-en | Fastest | Good | English only | Real-time English transcription |

## 🐛 Troubleshooting

### Microphone Not Working
- Check browser permissions
- Ensure you're using HTTPS or localhost
- Try a different browser

### API Errors
- Verify your API key is correct
- Check your Groq account has available credits
- Ensure stable internet connection

### No Transcription Appearing
- Check browser console for errors
- Verify audio is being recorded (check visualizer)
- Try a different audio input device

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [Groq](https://groq.com) for providing ultra-fast AI inference
- [OpenAI Whisper](https://openai.com/research/whisper) for the speech recognition model
- Web Audio API for audio processing capabilities

## 📧 Contact

Project Link: [https://github.com/your-username/tgh-speech-hearing](https://github.com/your-username/tgh-speech-hearing)

## 🗺️ Roadmap

- [ ] Add language selection
- [ ] Export transcriptions to file (TXT, JSON, SRT)
- [ ] Speaker diarization support
- [ ] Real-time streaming transcription
- [ ] Audio file upload support
- [ ] Translation features
- [ ] Custom vocabulary/terminology support

---

**Made with ❤️ by [Your Name]**
