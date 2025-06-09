# 🌐 Basic English Translator

![Basic English Translator](https://img.shields.io/badge/HTML-E34F26?&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-1572B6?&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?&logo=javascript&logoColor=black)
![Vercel](https://img.shields.io/badge/Vercel-000000?logo=vercel&logoColor=white&style=flat)

A simple, responsive web-based translator built with *vanilla HTML*, *CSS*, and *JavaScript*. Translate text between English and 9 other languages with a clean, user-friendly interface.


## ✨ Features

- **Multi-language Support**: Translate between 10 languages including English, Spanish, French, German, Italian, Portuguese, Russian, Japanese, Korean, and Chinese
- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Real-time Character Counter**: Track your input with a 500-character limit
- **Language Swap**: Quickly switch source and target languages with one click
- **Copy to Clipboard**: Easily copy translations for use elsewhere
- **Keyboard Shortcuts**: Speed up your workflow with handy shortcuts
- **Error Handling**: Graceful fallback with basic dictionary when API is unavailable
- **Loading States**: Visual feedback during translation process
- **Clean UI**: Modern, intuitive interface with smooth animations

## 🌐 Live Demo

Experience the live version of this project: [v0-new-project-dvlsj1ckq4c-f786hdb0r-nheljim-edis-projects.vercel.app](https://v0-new-project-dvlsj1ckq4c-f786hdb0r-nheljim-edis-projects.vercel.app/)

## 🚀 Deployment

As a beginner and just starting to learn, this project was generated using *V0* and deployed on *Vercel*. For more information on how to create and deploy projects with *v0*, visit [v0.dev](https://v0.dev).

## 🚀 Quick Start

### Option 1: Direct Download
1. Download all files (\`index.html\`, \`styles.css\`, \`script.js\`)
2. Open \`index.html\` in your web browser
3. Start translating!

### Option 2: Clone Repository
\`\`\`bash
git clone <repository-url>
cd basic-english-translator
\`\`\`

### Option 3: Live Server (Recommended for Development)
\`\`\`bash
# Using Python
python -m http.server 8000

# Using Node.js (if you have live-server installed)
npx live-server

# Using PHP
php -S localhost:8000
\`\`\`

Then open \`http://localhost:8000\` in your browser.

## 📖 How to Use

### Basic Translation
1. **Select Languages**: Choose your source language (what you're translating from) and target language (what you're translating to)
2. **Enter Text**: Type or paste text in the left textarea (up to 500 characters)
3. **Translate**: Click the "🔄 Translate" button or press \`Ctrl+Enter\`
4. **View Result**: Your translation appears in the right textarea

### Advanced Features

#### Language Swap
- Click the **⇄** button between the language selectors to instantly swap source and target languages along with their text

#### Copy Translation
- Click the **📋 Copy** button to copy the translation to your clipboard
- The button will show "✅ Copied!" for 2 seconds to confirm

#### Clear All
- Click the **🗑️ Clear** button to clear both input and output text
- Use keyboard shortcut \`Ctrl+K\` for quick clearing

#### Keyboard Shortcuts
- \`Ctrl+Enter\` (or \`Cmd+Enter\` on Mac): Translate text
- \`Ctrl+K\` (or \`Cmd+K\` on Mac): Clear all text

## 🌍 Supported Languages

| Language | Code | Native Name |
|----------|------|-------------|
| English | en | English |
| Spanish | es | Español |
| French | fr | Français |
| German | de | Deutsch |
| Italian | it | Italiano |
| Portuguese | pt | Português |
| Russian | ru | Русский |
| Japanese | ja | 日本語 |
| Korean | ko | 한국어 |
| Chinese | zh | 中文 |

## 🔧 Technical Details

### Architecture
- **Frontend**: Pure *HTML5*, *CSS3*, and *ES6+ JavaScript*
- **Translation API**: MyMemory Translation API (free, no API key required)
- **Fallback**: Basic dictionary for common words when API is unavailable
- **No Dependencies**: Works without any external libraries or frameworks

### File Structure
\`\`\`
basic-english-translator/
├── index.html          # Main HTML structure
├── styles.css          # All styling and responsive design
├── script.js           # JavaScript functionality
└── README.md           # This file
\`\`\`

### Browser Compatibility
- ✅ Chrome 60+
- ✅ Firefox 55+
- ✅ Safari 12+
- ✅ Edge 79+
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

### API Information
This translator uses the [MyMemory Translation API](https://mymemory.translated.net/):
- **Free to use**: No API key required
- **Rate limits**: 1000 requests per day for anonymous usage
- **Fallback**: Basic dictionary for offline/limited connectivity scenarios

## 🎨 Customization

### Changing Colors
Edit the CSS variables in \`styles.css\`:
\`\`\`css
:root {
  --primary-color: #667eea;
  --secondary-color: #764ba2;
  --text-color: #333;
  --border-color: #e1e5e9;
}
\`\`\`

### Adding Languages
1. Add the language option to both select elements in \`index.html\`:
\`\`\`html
<option value="language-code">Language Name</option>
\`\`\`

2. Add translations to the basic dictionary in \`script.js\`:
\`\`\`javascript
const basicDictionary = {
  hello: { 
    es: "hola", 
    fr: "bonjour", 
    "new-lang": "translation"
  }
}
\`\`\`

### Modifying Character Limit
Change the \`maxlength\` attribute in \`index.html\` and update the counter logic in \`script.js\`:
\`\`\`javascript
this.charCounter.textContent = \`\${currentLength}/1000\` // Change 500 to your limit
\`\`\`

## 🐛 Troubleshooting

### Translation Not Working
1. **Check Internet Connection**: The translator requires internet access for the API
2. **API Limits**: If you've exceeded daily limits, try again tomorrow
3. **Fallback Mode**: For common words, a basic dictionary translation may appear

### Copy Function Not Working
- **Modern Browsers**: Uses Clipboard API
- **Older Browsers**: Falls back to \`document.execCommand\`
- **HTTPS Required**: Clipboard API requires HTTPS in production

### Mobile Issues
- **Viewport**: Ensure proper viewport meta tag is present
- **Touch Targets**: All buttons are sized for touch interaction
- **Responsive**: Layout adapts to screen size automatically

## 🤝 Contributing

Contributions are welcome! Here are some ways you can help:

1. **Bug Reports**: Open an issue describing the problem
2. **Feature Requests**: Suggest new features or improvements
3. **Code Contributions**: Fork, make changes, and submit a pull request
4. **Documentation**: Help improve this README or add code comments

### Development Setup
1. Fork the repository
2. Create a feature branch: \`git checkout -b feature-name\`
3. Make your changes
4. Test thoroughly on different devices/browsers
5. Commit: \`git commit -m "Add feature description"\`
6. Push: \`git push origin feature-name\`
7. Create a Pull Request

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- **MyMemory Translation API** for providing free translation services
- **Modern CSS Grid and Flexbox** for responsive layout capabilities
- **Fetch API** for clean, promise-based HTTP requests

## 📞 Support

If you encounter any issues or have questions:

1. Check the [Troubleshooting](#🐛-troubleshooting) section
2. Search existing issues in the repository
3. Create a new issue with detailed information
4. Include browser version, device type, and steps to reproduce

---

**Made with ❤️ using vanilla HTML, CSS, and JavaScript**

*No frameworks, no dependencies, just pure web technologies!*
