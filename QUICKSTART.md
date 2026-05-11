# 🚀 Quick Start Guide

Get TGH - Target Speech Hearing up and running in 5 minutes!

## 🎯 Option 1: GitHub Pages (Recommended for Hosting)

The fastest way to get your own hosted version:

1. **Fork this repository** on GitHub
2. **Enable GitHub Pages**:
   - Go to Settings → Pages
   - Source: Deploy from a branch
   - Branch: `main` / `root`
   - Save
3. **Access your app** at: `https://your-username.github.io/tgh-speech-hearing/`

✅ **Done!** The GitHub Action will automatically deploy your site.

## 💻 Option 2: Local Development

For testing and development:

### Method A: Direct File Open
```bash
# Clone the repository
git clone https://github.com/your-username/tgh-speech-hearing.git
cd tgh-speech-hearing

# Open in browser
# Just double-click index.html or:
open index.html  # macOS
xdg-open index.html  # Linux
start index.html  # Windows
```

⚠️ **Note**: Microphone may not work with `file://` protocol. Use a local server instead:

### Method B: Python Server
```bash
# Python 3
python3 -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

Then open: `http://localhost:8000`

### Method C: Node.js Server
```bash
# Using npx (no installation needed)
npx http-server

# Or install globally
npm install -g http-server
http-server
```

### Method D: PHP Server
```bash
php -S localhost:8000
```

## 🔑 Get Your Groq API Key

1. Visit [console.groq.com](https://console.groq.com)
2. Sign up or log in
3. Go to "API Keys"
4. Click "Create API Key"
5. Copy your key (starts with `gsk_...`)

## ✅ First Use

1. **Open the app** (via GitHub Pages or local server)
2. **Paste your API key** in the input field
3. **Click "Start Recording"**
4. **Allow microphone access** when prompted
5. **Speak clearly** into your microphone
6. **Click "Stop"** when done
7. **View your transcription** below

## 🎨 Customization

### Change Colors
Edit `index.html` and find the gradient:
```css
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```

### Change Models
In the app, use the dropdown to select:
- **Whisper Large v3** - Best accuracy
- **Whisper Large v3 Turbo** - Faster
- **Distil Whisper** - English only, fastest

## 🐛 Troubleshooting

### Microphone Not Working
- ✅ Use HTTPS or localhost (not `file://`)
- ✅ Check browser permissions
- ✅ Try a different browser

### API Errors
- ✅ Verify API key is correct
- ✅ Check Groq console for credits
- ✅ Check browser console for details

### No Audio Visualization
- ✅ Check microphone is connected
- ✅ Verify browser supports Web Audio API
- ✅ Try a different audio input device

## 📱 Mobile Use

TGH works on mobile browsers:
- ✅ Safari (iOS)
- ✅ Chrome (Android)
- ✅ Firefox (Android)

**Note**: Mobile requires HTTPS (GitHub Pages provides this automatically)

## 🔐 Security Tips

- 🔒 Never commit API keys to git
- 🔒 Use environment variables in production
- 🔒 Consider a backend proxy for public deployments
- 🔒 Rotate API keys regularly

## 📚 Next Steps

- Read the full [README.md](README.md)
- Check [CONTRIBUTING.md](CONTRIBUTING.md) to contribute
- Review [SECURITY.md](SECURITY.md) for security best practices
- See [CHANGELOG.md](CHANGELOG.md) for version history

## 💡 Tips

- **Speak clearly** for best results
- **Reduce background noise** when possible
- **Try different models** for speed vs. accuracy trade-off
- **Use timestamps** to track when each recording was made

## ❓ Need Help?

- 📖 Check the [README](README.md)
- 🐛 [Report issues](https://github.com/your-username/tgh-speech-hearing/issues)
- 💬 [Start a discussion](https://github.com/your-username/tgh-speech-hearing/discussions)

---

**Happy Transcribing! 🎉**
