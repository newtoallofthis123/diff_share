# Diff Share

A simple, elegant web-based text comparison tool that allows you to compare two texts side-by-side and share the results via URL.

**Live Demo**: [diff.noobscience.in](https://diff.noobscience.in)

![Diff Share Screenshot](https://via.placeholder.com/800x400/0d1117/c9d1d9?text=Diff+Share+Screenshot)

## ( Features

- Side-by-Side Comparison**: Clean, GitHub-style diff view with syntax highlighting
- URL Sharing**: Share your diffs via compressed URLs (up to 64KB)
- Dark/Light Theme**: Toggle between dark and light modes with persistent preferences
- Responsive Design**: Works seamlessly on desktop and mobile devices
- Real-time Diffs**: Auto-generates diffs as you type (with debouncing)
- No Server Required**: Runs entirely in the browser - no data sent to servers
- Programmer-Friendly**: Monospace fonts and code-oriented styling
- One-Click Sharing**: Copy shareable URLs to clipboard instantly

## Quick Start

1. **Enter your texts**: Type or paste text into the two input areas
2. **View the diff**: The comparison appears automatically below
3. **Share**: Click "Share URL" to generate a shareable link
4. **Send**: Share the URL - recipients can view the diff instantly

## Technology Stack

- **Pure HTML/CSS/JavaScript** - No build process required
- **[jsdiff](https://github.com/kpdecker/jsdiff)** - Text diffing algorithm
- **[diff2html](https://github.com/rtfpessoa/diff2html)** - Beautiful diff visualization
- **[lz-string](https://github.com/pieroxy/lz-string)** - Text compression for URLs
- **[highlight.js](https://highlightjs.org/)** - Syntax highlighting

## Use Cases

- **Code Reviews**: Share code changes with colleagues
- **Documentation**: Compare different versions of text
- **Writing**: Track changes in articles or documents
- **Education**: Demonstrate differences in code or text
- **Debugging**: Compare outputs or configurations

## Installation

### Option 1: Direct Download
1. Download the `index.html` file
2. Open in any modern web browser
3. Start comparing texts immediately!

### Option 2: Clone Repository
```bash
git clone <repository-url>
cd diff_share
open index.html
```

### Option 3: Serve Locally
```bash
# Using Python 3
python -m http.server 8000

# Using Node.js
npx serve .

# Using PHP
php -S localhost:8000
```

## URL Format

Shareable URLs use the following format:
```
https://diff.noobscience.in#<compressed_text1>Ê<compressed_text2>
```

- Texts are compressed using LZ-String compression
- Diamond separator (Ê) distinguishes between the two texts
- URLs support up to 64KB of data in the fragment

## Themes

The application supports both light and dark themes:

- **Dark Theme**: Default GitHub-dark inspired theme
- **Light Theme**: Clean, bright theme for daytime use
- **Auto-Detection**: Respects system color scheme preferences
- **Persistent**: Theme choice saved in localStorage

## Browser Support

- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

## Privacy

- **No server-side processing** - everything runs in your browser
- **No data collection** - no analytics or tracking
- **No external dependencies** at runtime - all libraries loaded from CDN
- **URL sharing only** - data is encoded in the URL itself

## Contributing

Contributions are welcome! Please feel free to submit issues or pull requests.

### Development Setup
1. Clone the repository
2. Make your changes to `index.html`
3. Test in multiple browsers
4. Submit a pull request

## License

This project is open source and available under the [MIT License](LICENSE).

## Copyright

© 2024 [NoobScience](https://noobscience.in). All rights reserved.

---

**Made with by NoobScience**

For more projects and tools, visit [NoobScience](https://noobscience.in)
