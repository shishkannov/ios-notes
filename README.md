<div align="center">

# 📝 iOS Notes

**A beautiful, modern notes application with iOS-inspired design**

[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)](https://github.com/yourusername/ios-notes)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-yellow.svg)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![CSS](https://img.shields.io/badge/CSS-3-blue.svg)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![HTML](https://img.shields.io/badge/HTML-5-orange.svg)](https://developer.mozilla.org/en-US/docs/Web/HTML)

*A minimalist notes app built with vanilla JavaScript, featuring a clean iOS-inspired UI, dark/light themes, multilingual support, and intuitive note management.*

[Features](#-features) • [Demo](#-demo) • [Installation](#-installation) • [Usage](#-usage) • [Contributing](#-contributing)

</div>

---

## 🎯 Overview

iOS Notes is a lightweight, browser-based notes application that brings the elegance of iOS design to the web. Built entirely with vanilla JavaScript, HTML, and CSS - no frameworks, no dependencies, just pure code.

### ✨ Key Highlights

- 🎨 **iOS-Inspired Design** - Beautiful, clean interface inspired by Apple's Notes app
- 🌓 **Dark/Light Themes** - Automatic theme detection with manual toggle
- 🌍 **Multilingual** - English and Russian language support
- 📱 **Fully Responsive** - Optimized for all screen sizes
- 💾 **Local Storage** - All data stored locally in your browser
- ⚡ **Zero Dependencies** - No build process, no npm, just open and use

## ✨ Features

| Feature | Description |
|---------|-------------|
| 📌 **Pin Notes** | Pin important notes to keep them at the top |
| 🔍 **Smart Search** | Real-time search through all notes by title or content |
| 🎨 **Themes** | Light and dark themes with system preference detection |
| 🌐 **Multilingual** | English and Russian language support (easily extensible) |
| 📱 **Responsive Design** | Optimized for mobile, tablet, and desktop |
| 🎯 **Selection Mode** | Select multiple notes for batch operations |
| 📋 **View Modes** | Switch between list and gallery views |
| 💾 **Local Storage** | All data stored locally in your browser |
| ✨ **Smooth Animations** | Beautiful UI transitions and micro-interactions |
| 📅 **Smart Grouping** | Notes automatically grouped by time (Today, Yesterday, This Week, etc.) |
| 🔄 **Duplicate Notes** | Quickly duplicate any note |
| 🗑️ **Batch Delete** | Delete multiple notes at once |
| 📝 **Rich Editing** | Clean, distraction-free editing experience |

## 🖼️ Demo

> **Note:** Add screenshots here once you deploy the app or create a demo page.

### Screenshots

<div align="center">

| Light Theme | Dark Theme |
|------------|------------|
| ![Light Theme](screenshots/light-theme.png) | ![Dark Theme](screenshots/dark-theme.png) |

| List View | Gallery View |
|-----------|--------------|
| ![List View](screenshots/list-view.png) | ![Gallery View](screenshots/gallery-view.png) |

</div>

## 🚀 Getting Started

### Prerequisites

No dependencies required! Just a modern web browser.

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/ios-notes.git
```

2. Navigate to the project directory:
```bash
cd notes-app
```

3. Open `index.html` in your web browser.

That's it! The app runs entirely in the browser with no build process needed.

### Running Locally

You can run the app in several ways:

**Option 1: Direct file opening**
- Simply double-click `index.html` to open it in your default browser

**Option 2: Local server (recommended)**
- Using Python:
```bash
python -m http.server 8000
```
- Using Node.js (with http-server):
```bash
npx http-server
```
- Using PHP:
```bash
php -S localhost:8000
```

Then open `http://localhost:8000` in your browser.

## 📁 Project Structure

```
notes-app/
├── index.html          # Main HTML file
├── css/                # Stylesheets
│   ├── main.css       # Main CSS file (imports all modules)
│   ├── variables.css  # CSS variables and theme definitions
│   ├── base.css       # Base styles and reset
│   ├── components.css # Component styles (modals, buttons, cards, etc.)
│   ├── media-small-mobile.css # Styles for small mobile devices (≤480px)
│   ├── media-mobile.css # Styles for mobile devices (≤768px)
│   ├── media-tablet.css # Styles for tablet devices (769px-1024px)
│   ├── media-desktop.css # Styles for desktop devices (≥1025px)
│   └── media-landscape.css # Landscape orientation styles
├── js/                 # JavaScript modules
│   ├── state.js       # Application state management
│   ├── dom.js         # DOM element references
│   ├── localization.js # Internationalization (i18n)
│   ├── utils.js       # Utility functions (date formatting, text truncation, etc.)
│   ├── notes.js       # Note management (CRUD operations, rendering)
│   ├── ui.js          # UI components (modals, toasts, menus, selection mode)
│   └── main.js        # Application initialization and event handlers
├── README.md           # Project documentation
├── LICENSE             # MIT License
└── .gitignore          # Git ignore rules
```

### Module Descriptions

#### JavaScript Modules

- **`state.js`** - Manages global application state (notes array, current note ID, search query, language, view mode, selection mode)
- **`dom.js`** - Contains all DOM element references for easy access throughout the application
- **`localization.js`** - Handles translations and language switching (English/Russian)
- **`utils.js`** - Helper functions: HTML escaping, text truncation, date formatting, Russian pluralization
- **`notes.js`** - Core note functionality: CRUD operations, rendering, time-based grouping, note cards creation
- **`ui.js`** - UI components: toast notifications, modals, menus, theme switching, view mode, selection mode
- **`main.js`** - Application entry point: initialization, event handlers setup, periodic updates

#### CSS Modules

- **`variables.css`** - CSS custom properties for colors, spacing, and theme definitions
- **`base.css`** - Reset styles, base typography, scrollbar styling, container layout
- **`components.css`** - All component styles: header, notes, modals, toasts, menus, selection mode
- **`media-small-mobile.css`** - Responsive styles for small mobile devices (max-width: 480px)
- **`media-mobile.css`** - Responsive styles for mobile devices (max-width: 768px)
- **`media-tablet.css`** - Responsive styles for tablet devices (769px - 1024px)
- **`media-desktop.css`** - Responsive styles for desktop and large desktop devices (≥1025px)
- **`media-landscape.css`** - Landscape orientation styles for mobile devices
- **`main.css`** - Main file that imports all CSS modules in the correct order

## 🎯 Usage

### Creating Notes

1. Click the **+** button at the bottom of the screen
2. Enter a title and content
3. Click **Save**

### Editing Notes

- Click on any note card to open it for editing
- Make your changes and click **Save**

### Pinning Notes

1. Open a note for editing
2. Click the **Pin** button in the modal actions
3. Pinned notes appear at the top in a separate section

### Searching

- Type in the search bar to filter notes by title or content
- The search icon changes to a clear button (×) when there's text

### Selection Mode

1. Click the menu button (⋮) in the top right
2. Select **"Select"** option
3. Use checkboxes to select notes
4. Use **"Select all"** to select all visible notes
5. Use **"Deselect all"** to clear selection
6. Click **"Delete"** to remove selected notes
7. Click **"Done"** (checkmark icon) to exit selection mode

### View Modes

- **List View** - Single column layout
- **Gallery View** - Multi-column grid layout (2 columns on desktop)

Switch between modes via the menu (⋮) → **"Show as gallery"** / **"Show as list"**

### Themes

Toggle between light and dark themes via the menu (⋮) → **"Toggle theme"**

The app automatically detects your system theme preference on first load.

### Languages

Switch between English and Russian via the menu (⋮) → **"Switch language"**

## 🛠️ Technologies Used

- **HTML5** - Semantic markup
- **CSS3** - Modern styling with CSS variables, flexbox, and grid
- **Vanilla JavaScript** - No frameworks, pure ES6+
- **LocalStorage API** - Client-side data persistence

## 📱 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## 📐 Responsive Design

The app is fully responsive and optimized for all screen sizes:

- **Small Mobile** (≤480px) - Optimized layout with smaller fonts and spacing
- **Mobile** (≤768px) - Single column layout, full-width modals
- **Tablet** (769px-1024px) - Adjusted grid layout, medium-sized containers
- **Desktop** (≥1025px) - Full-width layout with optimal spacing
- **Large Desktop** (≥1440px) - Expanded layout with increased container width

All responsive styles are organized in separate CSS files for better maintainability.

## 🎨 Design Features

- **iOS-inspired UI** - Clean, modern interface
- **Glassmorphism** - Frosted glass effects on modals and buttons
- **Smooth Animations** - CSS transitions and keyframe animations
- **Responsive Design** - Mobile-first approach
- **Accessibility** - Semantic HTML and ARIA labels

## 📝 Notes Storage

All notes are stored locally in your browser's `localStorage`. Your data never leaves your device.

## 🔧 Customization

### Adding New Languages

Edit `js/localization.js` and add translations to the `translations` object:

```javascript
const translations = {
    en: { /* English translations */ },
    ru: { /* Russian translations */ },
    // Add your language here
    es: {
        title: 'Notas',
        // ... more translations
    }
};
```

### Changing Colors

Edit `css/variables.css` to customize the color scheme:

```css
:root {
    --accent: #007aff; /* Change accent color */
    --danger: #ff3b30;  /* Change danger color */
    /* ... */
}
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- Design inspired by iOS Notes app
- Icons from custom SVG designs
- Font stack: SF Pro Display, Segoe UI, Roboto

## 📊 Project Stats

- **Lines of Code:** ~1,200+ (JavaScript + CSS)
- **Modules:** 7 JavaScript modules, 9 CSS modules
- **Languages:** JavaScript, HTML, CSS
- **Dependencies:** None
- **Browser Support:** Modern browsers (Chrome, Firefox, Safari, Edge)

## 🌟 Star History

If you find this project useful, please consider giving it a ⭐ on GitHub!

## 📧 Contact & Support

- 🐛 **Found a bug?** [Open an issue](https://github.com/yourusername/ios-notes/issues)
- 💡 **Have a suggestion?** [Create a feature request](https://github.com/yourusername/ios-notes/issues)
- 🤝 **Want to contribute?** See [CONTRIBUTING.md](.github/CONTRIBUTING.md)

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

<div align="center">

**Made with ❤️ using vanilla JavaScript**

[⬆ Back to Top](#-ios-notes)

</div>

