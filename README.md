# PrecisionBooks Accounting - WordPress Demo Website

## Project Overview

This is a professional static HTML/CSS/JavaScript demo website for **PrecisionBooks Accounting Firm**, created as a portfolio piece for a WordPress website redesign project.

**Live Demo:** [https://phoenixflix.vercel.app/AccFirmDemo](https://phoenixflix.vercel.app/AccFirmDemo)
**Standalone Demo:** https://phoenixflix.vercel.app/AccountingFirmDemo/

### Purpose
- Demonstrate UI/UX design skills for job application
- Showcase modern, professional design aesthetic for accounting/financial services
- Provide a foundation that can be migrated to WordPress

## Features

### Pages Included
1. **Landing Page** (`index.html`) - Hero section, services overview, why choose us, process timeline, CTA
2. **Accounting Services** (`accounting-services.html`) - Detailed service breakdown with sidebar
3. **Contact** (`contact.html`) - Contact form and business information
4. **Additional pages** (placeholders ready): Tax Agent, Corporate Registration, Business Intelligence, Case Studies

### Design System

**Color Palette:**
- Primary: #2774AE (Rich Cerulean) - Professional, trustworthy blue
- Primary Dark: #00416A (Yale Blue) - Deep, prestigious
- Secondary: #708090 (Slate Grey) - Sophisticated, balanced
- Accent: #D4A574 (Warm gold) - Premium touch

**Typography:**
- Headers: Montserrat (professional, geometric, modern)
- Body: Open Sans (friendly, readable, accessible)

**Design Approach:**
- Clean, professional corporate aesthetic
- Generous whitespace for clarity
- Modern card-based layouts
- Smooth transitions and hover effects
- Fully responsive design

## Technologies Used

- **HTML5** - Semantic markup
- **CSS3** - Custom properties (CSS variables), Grid, Flexbox
- **Vanilla JavaScript** - No frameworks, lightweight interactions
- **Tabler Icons** - Professional icon set via CDN
- **Google Fonts** - Montserrat & Open Sans

## File Structure

```
accounting-firm-demo/
├── index.html                  # Landing page
├── accounting-services.html    # Accounting services detail page
├── contact.html               # Contact page
├── css/
│   ├── variables.css          # Design tokens & CSS variables
│   ├── base.css              # Reset & typography
│   ├── components.css        # Reusable components
│   ├── layout.css            # Navigation, hero, footer
│   └── pages.css             # Page-specific styles
├── js/
│   └── main.js               # Interactive features
└── README.md                 # This file
```

## Setup & Usage

1. **Open in browser**: Simply open `index.html` in any modern web browser
2. **No build process required**: All assets loaded via CDN
3. **Live server recommended**: Use VS Code Live Server or similar for best development experience

## Key Features

### Navigation
- Sticky header with scroll effect
- Mobile-responsive hamburger menu
- Active page highlighting

### Hero Section
- Full-screen hero with overlay
- Animated statistics counter
- Dual CTA buttons
- Parallax background effect

### Components
- Service cards with hover animations
- Feature lists with icons
- Timeline component for process
- Image stack with decorative background
- Gradient CTA cards
- Responsive contact form

### Interactions
- Smooth scroll navigation
- Intersection Observer animations
- Form validation
- Mobile menu toggle
- Counter animations

## WordPress Migration Notes

This demo is designed to be easily migrated to WordPress:

1. **Component-based structure** - Each section can become a Gutenberg block or widget
2. **Consistent design system** - CSS variables make theming straightforward
3. **Semantic HTML** - Clean structure for WordPress templates
4. **Mobile-first responsive** - Works across all devices
5. **SEO-friendly** - Proper heading hierarchy, meta tags, semantic markup

## Customization

### Colors
Edit `css/variables.css` - all colors defined as CSS custom properties

### Typography
Change Google Fonts import in HTML `<head>` and update font variables in `css/variables.css`

### Content
All content is in HTML files - easily editable text, images, and structure

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Credits

**Design & Development**: Portfolio demo piece
**Images**: Unsplash & Pexels (with attribution)
**Icons**: Tabler Icons
**Fonts**: Google Fonts (Montserrat, Open Sans)

## License

Distributed under the MIT License. See `license` for more information.

This is a demo project created for portfolio/job application purposes.

---

**Note**: This is a static prototype. For production use, implement:
- Backend form handling
- Content Management System (WordPress)
- Analytics integration
- Performance optimization
- Security headers
- SSL certificate
