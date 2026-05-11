# Security Policy

## Supported Versions

| Version | Supported          |
| ------- | ------------------ |
| 1.0.x   | :white_check_mark: |

## Reporting a Vulnerability

We take the security of TGH - Target Speech Hearing seriously. If you discover a security vulnerability, please follow these steps:

### How to Report

1. **DO NOT** open a public issue
2. Email the maintainer directly (add your email here)
3. Provide detailed information about the vulnerability:
   - Type of vulnerability
   - Steps to reproduce
   - Potential impact
   - Suggested fix (if any)

### What to Expect

- **Acknowledgment**: Within 48 hours
- **Initial Assessment**: Within 5 business days
- **Regular Updates**: Every 7 days until resolved
- **Fix Timeline**: Depends on severity
  - Critical: 1-7 days
  - High: 7-30 days
  - Medium: 30-90 days
  - Low: Best effort basis

### Security Best Practices

When using TGH:

1. **API Keys**
   - Never commit API keys to version control
   - Use environment variables in production
   - Rotate keys regularly
   - Monitor API usage for anomalies

2. **HTTPS**
   - Always use HTTPS in production
   - Microphone access requires secure context
   - GitHub Pages provides HTTPS by default

3. **Client-Side Security**
   - API keys stored in localStorage are accessible to JavaScript
   - Consider using backend proxy for production deployments
   - Implement rate limiting if self-hosting

4. **Audio Data**
   - Audio is sent directly to Groq API
   - No audio is stored on our servers
   - Review Groq's privacy policy for their data handling

5. **Browser Permissions**
   - Request microphone access only when needed
   - Explain permission requirements to users
   - Handle permission denials gracefully

## Disclosure Policy

- We follow responsible disclosure practices
- Security researchers will be credited (if desired)
- Coordinated public disclosure after fix is available
- CVE IDs will be requested for significant vulnerabilities

## Security Updates

Security updates will be:
- Released as patch versions (e.g., 1.0.1)
- Documented in CHANGELOG.md
- Announced in release notes
- Tagged with `security` label

## Known Limitations

1. **Local Storage**: API keys in localStorage are accessible to JavaScript running on the same domain
2. **Client-Side Only**: No server-side validation or rate limiting
3. **Browser Security**: Relies on browser's same-origin policy

## Security Considerations for Self-Hosting

If you're hosting TGH yourself:

1. **Use a Backend Proxy**
   ```javascript
   // Instead of calling Groq API directly
   // Proxy through your backend
   fetch('https://your-backend.com/api/transcribe', {
       // Your API key stays server-side
   });
   ```

2. **Implement Rate Limiting**
   - Prevent API abuse
   - Monitor usage patterns
   - Set per-user quotas

3. **Content Security Policy**
   ```html
   <meta http-equiv="Content-Security-Policy" 
         content="default-src 'self'; 
                  connect-src 'self' https://api.groq.com;">
   ```

4. **CORS Configuration**
   - Restrict allowed origins
   - Use specific domains, not wildcards

## Contact

For security concerns: [Add contact method]

For general questions: Use GitHub Issues

---

**Last Updated**: May 10, 2026
