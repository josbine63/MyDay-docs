# MyDay Documentation - Multilingual Site

## Structure

```
/
├── index.html          # Language selector page (landing page)
├── styles.css          # Shared CSS styles
├── script.js           # Shared JavaScript
├── Icon-App.png        # App icon
├── en/                 # English version
│   └── index.html      # English content
├── fr/                 # French version
│   └── index.html      # French content
└── README.md           # This file
```

## How It Works

### Language Selection
- The root `index.html` serves as a language selector
- Users can choose between English (🇬🇧) and French (🇫🇷)
- Language preference is saved in localStorage for future visits
- Auto-detection based on browser language is available but commented out by default

### Navigation Between Languages
- Each language page has a language switcher in the navigation menu
- FR page: Click "🇬🇧 EN" to switch to English
- EN page: Click "🇫🇷 FR" to switch to French

### Shared Resources
- CSS, JavaScript, and images are stored at the root level
- Both language versions reference these shared files using relative paths (`../`)

## Deployment to GitHub Pages

1. Push the entire `MyDay-docs-multilang` folder contents to your GitHub repository
2. Enable GitHub Pages in repository settings
3. Set the source to the main/master branch, root directory
4. Your site will be available at: `https://yourusername.github.io/MyDay-docs/`

## Customization

### Enable Auto Language Detection
In `index.html`, uncomment the JavaScript code block to enable automatic redirection based on browser language:

```javascript
const userLang = navigator.language || navigator.userLanguage;
// ... rest of the code
```

### Adding New Languages
1. Create a new folder (e.g., `es/` for Spanish)
2. Copy one of the existing language `index.html` files
3. Translate the content
4. Update the language selector in `index.html` to include the new language
5. Add language switcher links to all language versions

## Local Testing

To test locally:
1. Open `index.html` in a web browser
2. Select your language
3. Navigate the site and test the language switcher

## Notes

- All translations maintain the same structure and styling
- The French version is the original, English is the translation
- Mobile responsive design is preserved across all languages
- No build process required - pure HTML/CSS/JS

---

Created: January 2026
Last Updated: January 2026
