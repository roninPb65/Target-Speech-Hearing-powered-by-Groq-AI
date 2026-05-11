# Contributing to TGH - Target Speech Hearing

Thank you for your interest in contributing to TGH! We welcome contributions from the community.

## 🤝 How to Contribute

### Reporting Bugs

If you find a bug, please create an issue with:

- Clear title and description
- Steps to reproduce
- Expected vs actual behavior
- Browser and OS information
- Screenshots if applicable

### Suggesting Features

Feature suggestions are welcome! Please:

- Check if the feature has already been suggested
- Provide a clear use case
- Explain why it would benefit users
- Consider implementation complexity

### Pull Requests

1. **Fork the Repository**
   ```bash
   git clone https://github.com/your-username/tgh-speech-hearing.git
   cd tgh-speech-hearing
   ```

2. **Create a Branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```

3. **Make Your Changes**
   - Follow the existing code style
   - Test thoroughly in multiple browsers
   - Update documentation if needed

4. **Commit Your Changes**
   ```bash
   git commit -m "Add: brief description of changes"
   ```
   
   Use conventional commit messages:
   - `Add:` for new features
   - `Fix:` for bug fixes
   - `Update:` for updates to existing features
   - `Refactor:` for code refactoring
   - `Docs:` for documentation changes

5. **Push to Your Fork**
   ```bash
   git push origin feature/your-feature-name
   ```

6. **Create Pull Request**
   - Provide clear description of changes
   - Reference any related issues
   - Include screenshots for UI changes

## 📝 Code Style Guidelines

### JavaScript

- Use ES6+ features
- Use `const` and `let`, avoid `var`
- Use meaningful variable names
- Add comments for complex logic
- Keep functions focused and small

Example:
```javascript
// Good
const transcribeAudio = async (audioBlob) => {
    // Implementation
};

// Avoid
var x = function(y) { /* ... */ };
```

### HTML

- Use semantic HTML5 elements
- Keep structure clean and accessible
- Add ARIA labels where appropriate

### CSS

- Use consistent naming conventions
- Group related styles together
- Add comments for complex sections
- Prefer flexbox/grid over floats

## 🧪 Testing

Before submitting:

- [ ] Test in Chrome, Firefox, and Safari
- [ ] Test on mobile devices
- [ ] Verify microphone permissions work
- [ ] Check API integration works correctly
- [ ] Ensure no console errors
- [ ] Test with different audio inputs

## 📚 Documentation

Update documentation when:

- Adding new features
- Changing existing functionality
- Fixing bugs that affect usage
- Adding configuration options

## 🎯 Priority Areas

We're especially interested in contributions for:

- Browser compatibility improvements
- Accessibility enhancements
- Performance optimizations
- UI/UX improvements
- Additional language support
- New transcription features

## ❓ Questions?

Feel free to:

- Open an issue for discussion
- Reach out via GitHub Discussions
- Check existing issues and PRs

## 📜 Code of Conduct

- Be respectful and inclusive
- Provide constructive feedback
- Focus on what's best for the project
- Welcome newcomers

Thank you for contributing! 🙏
