# HTML Template Editor

A powerful and user-friendly GUI application for editing HTML templates without coding knowledge. Built with Python and CustomTkinter, this tool allows users to easily modify text content, images, and links in HTML files through an intuitive interface.

## Features

### 🎯 **Multi-Tab Interface**
- **Text Editing Tab**: Edit all text elements (headings, paragraphs, links, buttons, etc.)
- **Image Editing Tab**: Manage images with preview, upload, and URL support
- **Link Editing Tab**: Modify hyperlinks, display text, and link properties

### 📝 **Text Editing**
- Automatically detects and lists all editable text elements
- Supports various HTML tags: `title`, `h1-h6`, `p`, `span`, `div`, `a`, `button`, `label`, `li`, `td`, `th`
- Smart input fields: single-line for short text, multi-line for longer content
- Vietnamese tag descriptions for better understanding

### 🖼️ **Image Management**
- Live image preview with thumbnail generation
- Upload images from local computer (auto-converts to base64)
- Support for various image formats: PNG, JPG, JPEG, GIF, BMP, WebP
- Edit image attributes: `src`, `alt`, `title`
- Handle both local files and web URLs
- Base64 embedded image support

### 🔗 **Link Editing**
- Edit link text and URL destinations
- Modify link titles and target attributes
- Dropdown selection for common target values (`_blank`, `_self`, etc.)
- Support for both internal and external links

### 🛠️ **Advanced Features**
- **Live Preview**: Built-in Flask server for real-time HTML preview in browser
- **Command Line Support**: Open HTML files directly from command line
- **Multiple Save Options**: Save to original file or save as new file
- **Smooth Scrolling**: Optimized mouse wheel and touchpad support
- **Error Handling**: Comprehensive error handling with user-friendly messages
- **Cross-Platform**: Works on Windows, macOS, and Linux

## Installation

### Prerequisites
- Python 3.7 or higher
- Required Python packages (install via pip):

```bash
pip install customtkinter tkinter beautifulsoup4 flask pillow
```

### Quick Install
1. Download the `simple-website-editor.py` file
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the application:
   ```bash
   python simple-website-editor.py
   ```

### Command Line Usage
You can also open HTML files directly:
```bash
python simple-website-editor.py path/to/your/file.html
```

## Usage Guide

### Getting Started
1. **Launch the application**
2. **Select HTML File**: Click "Choose HTML File" or drag and drop an HTML file
3. **Edit Content**: Use the tabs to modify different aspects of your HTML:
   - **Text Tab**: Edit headings, paragraphs, and other text content
   - **Image Tab**: Replace images, edit alt text, and titles
   - **Link Tab**: Modify links, URLs, and link properties

### Text Editing
- Each text element is displayed with its HTML tag type and Vietnamese description
- Short text uses single-line input fields
- Long text (>100 characters) uses multi-line text areas
- Changes are applied in real-time when you save

### Image Editing
- **Preview**: See thumbnail previews of all images
- **Upload**: Click "Choose image from computer" to upload new images
- **URL Preview**: Click "Preview URL" to load images from web URLs
- **Attributes**: Edit alt text and title attributes for accessibility

### Link Editing
- **Display Text**: Edit the text that appears as the clickable link
- **URL**: Modify where the link points to
- **Title**: Add hover text for the link
- **Target**: Choose how the link opens (same window, new window, etc.)

### Saving and Preview
- **Save**: Overwrite the original HTML file
- **Save As**: Create a new HTML file with your changes
- **Preview**: Launch a local server to preview your changes in a web browser

## Technical Details

### Architecture
- **GUI Framework**: CustomTkinter (dark theme, modern UI)
- **HTML Parsing**: BeautifulSoup4 for robust HTML manipulation
- **Image Processing**: PIL (Pillow) for image handling and thumbnails
- **Preview Server**: Flask for local development server
- **Threading**: Separate threads for non-blocking operations

### File Support
- **HTML Files**: Standard HTML files with UTF-8 encoding
- **Image Formats**: PNG, JPG, JPEG, GIF, BMP, WebP
- **Image Embedding**: Automatic base64 conversion for uploaded images
- **Encoding**: Full UTF-8 support for international characters

### Compatibility
- **Python**: 3.7+
- **Operating Systems**: Windows 10+, macOS 10.14+, Linux (Ubuntu 18.04+)
- **Browsers**: All modern browsers for preview functionality

## Troubleshooting

**Application won't start:** Ensure all dependencies are installed and Python 3.7+ is used.

**Images not loading:** Check file paths are correct and image files exist.

**Preview not working:** Ensure port 5000 is available and Flask is installed.

## Development

### Contributing
1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

### Future Enhancements
- [ ] CSS styling editor
- [ ] Form elements editing
- [ ] Undo/Redo functionality
- [ ] Multi-file project support
- [ ] Template library
- [ ] Export to different formats

## License

This project is licensed under the GNU General Public License v3.0 - see the [LICENSE](LICENSE) file for details.

This means you can freely use, modify, and distribute this software, but any derivative work must also be licensed under GPL v3.

## Support

For issues, feature requests, or questions:
1. Check the troubleshooting section above
2. Review existing issues in the repository
3. Create a new issue with detailed information about your problem

## Changelog

### Version 1.0.0
- Initial release
- Text editing functionality
- Image management with preview
- Link editing capabilities
- Live preview server
- Command line support
- Cross-platform compatibility

---

**Made with ❤️ for easy HTML editing**
