# Newsletter Preview Analyzer

A simple, browser-based tool that helps email marketers and developers visualize how their newsletters will appear in different email clients. The tool provides instant preview of subject lines and preview text in both desktop and mobile email client layouts.

![Newsletter Preview Analyzer](https://via.placeholder.com/800x400)

## Features

- **Subject Line Input**: Manually enter subject lines or auto-extract from newsletter HTML
- **HTML Analysis**: Paste your newsletter HTML to automatically extract preview text
- **Live Preview**: Real-time updates as you modify content
- **Multi-Format Display**:
  - Desktop email client preview
  - Mobile email client preview
  - Raw preview text display
- **Dark Mode**: Easy on the eyes with a professional dark theme

## Installation

1. Clone this repository:
```bash
git clone https://github.com/aghorilabs/newsletter-preview-analyzer.git
```

2. No additional dependencies required! Simply open `index.html` in a web browser.

## Usage

1. **Enter Subject Line**:
   - Type your subject line in the top input field
   - Or let it auto-populate from your newsletter HTML

2. **Paste Newsletter HTML**:
   - Paste your complete newsletter HTML into the textarea
   - The tool will automatically extract preview text

3. **View Previews**:
   - See how your newsletter appears in desktop email clients
   - Check the mobile preview for smaller screens
   - Review the raw preview text

## How It Works

The analyzer looks for preview text in the following locations:

### Subject Line Detection
- `<meta name="subject">` tags
- `<meta name="og:title">` tags
- `<title>` elements
- Manual input (overrides detected values)

### Preview Text Detection
- `<meta name="description">` tags
- `<meta name="preview">` tags
- `<div data-preview-text>` elements
- Falls back to first paragraph text if no meta tags found

## Browser Support

Tested and working in:
- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Customization

### Modifying Colors
The tool uses CSS variables for easy theme customization. Edit these variables in the `:root` selector:

```css
:root {
    --bg-primary: #1a1a1a;
    --bg-secondary: #242424;
    --bg-tertiary: #2d2d2d;
    --text-primary: #ffffff;
    --text-secondary: #b3b3b3;
    --border-color: #333333;
    --accent-color: #4a9eff;
}
```

### Preview Layouts
You can customize the preview layouts by modifying the HTML structure within:
- `.desktop-preview` for desktop layout
- `.mobile-preview` for mobile layout

## Contributing

1. Fork the repository
2. Create your feature branch: `git checkout -b feature/my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin feature/my-new-feature`
5. Submit a pull request

## License

This project is licensed under the MIT License - see the LICENSE.md file for details

## Author

Your Name
- Website: [http://aghori-labs.com/](https://http://aghori-labs.com/)
- GitHub: [@aghorilabs](https://github.com/aghorilabs)

## Acknowledgments

- Inspired by email client preview displays
- Built with vanilla HTML, CSS, and JavaScript
- Uses system font stack for optimal performance

## Support

For support, please open an issue in the GitHub repository or contact [aghorilabs@gmail.com](mailto:aghorilabs@gmail.com)