# Docusaurus Template for QuantCDN

[![Deploy to QuantCDN](https://www.quantcdn.io/img/quant-deploy-btn-sml.svg)](https://dashboard.quantcdn.io/deploy/static/ssg-docusaurus)

A modern documentation site template using [Docusaurus](https://docusaurus.io/), the documentation framework from Meta. Optimized for deployment on QuantCDN.

## Features

- **MDX Support** - Write interactive documentation with React components
- **Versioning** - Built-in support for documentation versioning
- **i18n** - Internationalization support for multiple languages
- **Search** - Easy integration with search providers
- **Blog** - Built-in blog functionality
- **Dark Mode** - Automatic dark mode support

## Quick Start

### Prerequisites

- Node.js 18.0 or higher
- npm or yarn

### Installation

```bash
npm install
```

### Development

Start the development server:

```bash
npm start
```

This opens your browser at `http://localhost:3000`.

### Build

Build the site for production:

```bash
npm run build
```

The static files are generated in the `build` directory.

### Preview Production Build

```bash
npm run serve
```

## Project Structure

```
ssg-docusaurus/
├── blog/                    # Blog posts
│   └── welcome.md
├── docs/                    # Documentation pages
│   └── intro.md
├── src/
│   ├── css/
│   │   └── custom.css      # Custom styles
│   └── pages/
│       └── index.js        # Homepage
├── static/                  # Static assets
├── docusaurus.config.js     # Site configuration
├── sidebars.js              # Sidebar configuration
└── package.json
```

## Deployment to QuantCDN

### Automatic Deployment

This template includes a GitHub Actions workflow (`.github/workflows/deploy.yml`) that automatically deploys your site when you push to the main branch.

### Required Secrets

Configure these secrets in your GitHub repository settings:

| Secret | Description |
|--------|-------------|
| `QUANT_CUSTOMER` | Your QuantCDN customer ID |
| `QUANT_PROJECT` | Your QuantCDN project name |
| `QUANT_TOKEN` | Your QuantCDN API token |

## Configuration

### Site Configuration

Edit `docusaurus.config.js` to customize:

- Site title and tagline
- URL and base URL
- Navbar items
- Footer links
- Theme colors

### Sidebar Configuration

Edit `sidebars.js` to organize your documentation structure.

### Custom CSS

Add custom styles in `src/css/custom.css`.

## Adding Content

### Documentation

Add Markdown or MDX files to the `docs/` directory. Use front matter for metadata:

```md
---
sidebar_position: 1
title: My Page Title
---

# My Page

Content here...
```

### Blog Posts

Add blog posts to the `blog/` directory with the format `YYYY-MM-DD-title.md`:

```md
---
slug: my-post
title: My Blog Post
authors: [default]
tags: [tag1, tag2]
---

Post content...
```

## Resources

- [Docusaurus Documentation](https://docusaurus.io/docs)
- [QuantCDN Documentation](https://docs.quantcdn.io/)
- [MDX Documentation](https://mdxjs.com/)

## License

MIT
