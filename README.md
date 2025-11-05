# Days I've Been Single

A minimalist, terminal-style single-page website that displays a real-time counter showing how many days you've been single. Built with Eleventy and Tailwind CSS, featuring a sleek terminal aesthetic with live-updating counters.

## Features

- **Real-time Counter**: Automatically updates every second with days, hours, minutes, and seconds
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

3. Update the start date in `src/index.njk`:
```njk
{% set startDate = "2024-04-25" %}
```

And in the JavaScript section:
```javascript
const startDate = new Date('2024-04-25T00:00:00');
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

## Customization

### Change the Start Date

Edit the date in two places in `src/index.njk`:
1. Line 6: `{% set startDate = "2024-04-25" %}`
2. Line 118: `const startDate = new Date('2024-04-25T00:00:00');`

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

