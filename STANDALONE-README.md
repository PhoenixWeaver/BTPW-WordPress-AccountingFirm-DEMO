# PrecisionBooks Accounting - Standalone Demo

## Overview
This is a completely **independent, standalone website** for a professional accounting firm. It shares the same domain as PhoenixFlix but operates entirely independently.

## File Structure
```
AccountingFirmDemo/
├── index.html                # Main homepage (fully self-contained)
├── css/
│   ├── variables.css         # Design tokens & CSS variables
│   ├── base.css             # Base styles & typography
│   ├── components.css       # Reusable UI components
│   ├── layout.css           # Navigation, hero, footer layouts
│   └── pages.css            # Page-specific styles
├── js/
│   └── main.js              # Navigation, animations, interactions
└── STANDALONE-README.md     # This file
```

## Features
- ✅ **Fully Independent**: No dependencies on PhoenixFlix app
- ✅ **Self-Contained**: All CSS and JavaScript files are local
- ✅ **Responsive Design**: Mobile-first, works on all devices
- ✅ **Modern UI**: Professional blue & grey color palette
- ✅ **Interactive**: Smooth animations, scroll effects, mobile menu
- ✅ **Single Page**: All navigation links point to sections on the same page

## External Dependencies
The only external resources are CDN-based:
- **Tabler Icons**: Icon library (https://cdn.jsdelivr.net/npm/@tabler/icons-webfont)
- **Google Fonts**: Montserrat & Open Sans fonts
- **Unsplash Images**: Stock photography for hero and content sections

## How to Use

### Local Development
Simply open `AccFirmDemo.html` in a web browser:
```bash
# Navigate to the directory
cd AccountingFirmDemo

# Open in browser (Windows)
start index.html

# Or double-click the file in File Explorer
```

### Deployment

**GitHub + Vercel Setup:**
1. The `Accounting-firm-demo` folder is located in `public/Accounting-firm-demo/`
2. Push your repository to GitHub: https://github.com/PhoenixWeaver/BTPW_Phoenixflix
3. Vercel automatically deploys from the `public/` directory
4. Access the accounting demo at: **https://phoenixflix.vercel.app/AccFirmDemo**

The `vercel.json` configuration includes a rewrite rule that maps `/AccFirmDemo` to `/Accounting-firm-demo/index.html`.

**Alternative Access:**
- Direct path: https://phoenixflix.vercel.app/AccountingFirmDemo/

**Other Deployment Options:**
Upload the entire `AccountingFirmDemo` folder to your web server. The page will work independently at any URL path.

### Customization

#### Colors
Edit `css/variables.css` to change the color scheme:
```css
--color-primary: #2774AE;        /* Main brand color */
--color-primary-light: #5EA5DB;  /* Lighter variant */
--color-primary-dark: #00416A;   /* Darker variant */
```

#### Content
Edit `AccFirmDemo.html` to update:
- Company name and tagline
- Service descriptions
- Contact information
- Statistics and testimonials

#### Images
Replace Unsplash URLs with your own images or use the stock_search functionality.

## Navigation Structure
All navigation links point to sections on the same page:
- **Home** → `#home` (Hero section)
- **Services** → `#services` (Services overview)
- **Process** → `#process` (How we work)
- **Contact** → `#contact` (Contact form/CTA)

## Browser Compatibility
- ✅ Chrome/Edge (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Mobile browsers (iOS Safari, Chrome Android)

## Notes
- The page uses modern CSS features (CSS Grid, CSS Variables, Backdrop Filter)
- JavaScript is vanilla (no frameworks/libraries needed)
- Images are loaded from Unsplash with proper attribution
- All interactions work without a backend (forms show alerts for demo purposes)

## License
See LICENSE file in the parent directory.

## 1. Build Script is Targeted
Looking at your FULL_build-optimized-clean.ps1:

Lines 78-81: It only minifies specific PhoenixFlix files:
public/styles.css
public/Newstyles.css
public/app.js
public/sw.js
It does NOT recursively minify everything in public/
The accounting demo files in public/Accounting-firm-demo/ are completely ignored
2. Separate File Loading
When users visit phoenixflix.vercel.app/ → Only PhoenixFlix assets load
When users visit phoenixflix.vercel.app/AccFirmDemo → Only accounting demo assets load
No cross-contamination - browsers only request files for the current page
3. Independent Assets
public/
├── app.js              ← PhoenixFlix (minified by script)
├── styles.css          ← PhoenixFlix (minified by script)
├── Newstyles.css       ← PhoenixFlix (minified by script)
└── Accounting-firm-demo/
    ├── css/            ← Separate, NOT touched by build script
    └── js/             ← Separate, NOT touched by build script
4. Size Impact
The accounting demo adds:

~50KB of CSS files
~5KB of JavaScript
Only loaded when someone visits /AccFirmDemo
Zero impact on PhoenixFlix page load times
5. Vercel Optimization
Vercel automatically:

Serves each file separately with proper caching
Compresses assets with gzip/brotli
Only delivers what's requested per route

Summary:

🎯 The PhoenixFlix app performance remains exactly the same

Build time: No change (script ignores accounting demo)
Load time: No change (separate routes, separate assets)
Binary size: No change (Go backend doesn't include frontend files)
Minification: Only PhoenixFlix files are minified as before
The accounting demo is like having two completely separate websites that just happen to share the same domain! 🚀
