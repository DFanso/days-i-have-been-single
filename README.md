# Days I Was Single

A minimalist, terminal-style single-page website that displayed a real-time counter showing how many days I was single. The timer has been **stopped** — it ran from April 25, 2024 to February 7, 2026 (653 days). Built with Eleventy and Tailwind CSS, featuring a sleek terminal aesthetic.

## Features

- **Frozen Counter**: Final count locked at 653 days, with confetti celebration
- **Terminal UI**: Beautiful terminal-inspired design with syntax highlighting aesthetics
- **Responsive Design**: Fully responsive and mobile-friendly
- **Additional Stats**: Shows weeks, months, and years equivalent
- **Zero Dependencies**: No JavaScript frameworks, just vanilla JS
- **Static Site**: Fast and lightweight, built with Eleventy

## Getting Started

### Prerequisites

- Node.js (v16 or higher)
- pnpm (or npm/yarn)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/dfanso/days-i-have-been-single.git
cd days-i-have-been-single
```

2. Install dependencies:
```bash
pnpm install
```

3. The timer is currently stopped at February 7, 2026. To modify dates, edit `src/index.njk`:
```njk
{% set startDate = "2024-04-25" %}
{% set endDate = "2026-02-07" %}
```

And in the JavaScript section:
```javascript
const startDate = new Date('2024-04-25T00:00:00');
const endDate = new Date('2026-02-07T12:00:00');
```

4. Build the project:
```bash
pnpm run build
```

5. Start the development server:
```bash
pnpm run dev
```

The site will be available at `http://localhost:3000`

## Available Scripts

- `pnpm run build` - Build CSS and generate static site
- `pnpm run dev` - Build CSS and start development server with watch mode
- `pnpm run build:css` - Build Tailwind CSS only
- `pnpm run watch:css` - Watch and rebuild CSS on changes
- `pnpm run build:eleventy` - Build Eleventy site only
- `pnpm run watch:eleventy` - Start Eleventy development server

## Tech Stack

- **[Eleventy](https://www.11ty.dev/)** - Static site generator
- **[Tailwind CSS](https://tailwindcss.com/)** - Utility-first CSS framework
- **Vanilla JavaScript** - No frameworks, just pure JS
- **[Vercel Analytics](https://vercel.com/analytics)** - Web analytics

## Analytics

This project includes Vercel Analytics for tracking page views and user interactions. Analytics is automatically enabled when deployed to Vercel. For other hosting platforms, the analytics script is included via CDN and will work once the site is deployed.

To view analytics data:
1. Deploy your site to Vercel
2. Visit your Vercel dashboard
3. Navigate to the Analytics tab for your project

## Customization

### Change the Dates

The timer is frozen with a start and end date. Edit in `src/index.njk`:
1. Nunjucks variables: `{% set startDate = "2024-04-25" %}` and `{% set endDate = "2026-02-07" %}`
2. JavaScript: `const startDate = new Date('2024-04-25T00:00:00');` and `const endDate = new Date('2026-02-07T12:00:00');`

### Customize Colors

Modify the color scheme in `src/index.njk` by changing Tailwind classes:
- Terminal colors: `bg-gray-900`, `bg-gray-800`
- Accent colors: `text-cyan-400`, `text-blue-500`, `text-purple-500`

### Modify Layout

Edit `src/_layouts/base.njk` to change the overall page structure and add meta tags.

## License

ISC

## Author

DFanso - [Instagram](https://www.instagram.com/dfansoo/)

---

Built with Eleventy and Tailwind CSS

