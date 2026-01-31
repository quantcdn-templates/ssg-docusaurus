---
sidebar_position: 1
---

# Welcome to Your Documentation

Welcome to your new Docusaurus documentation site! This template is configured for deployment on **QuantCDN**.

## Getting Started

Get started by **editing this page** in `docs/intro.md`.

### What you'll need

- [Node.js](https://nodejs.org/en/download/) version 18.0 or above
- A text editor or IDE of your choice

## Project Structure

```
ssg-docusaurus/
├── docs/           # Documentation pages (Markdown/MDX)
├── blog/           # Blog posts
├── src/
│   ├── css/        # Custom CSS
│   └── pages/      # Custom React pages
├── static/         # Static assets
└── docusaurus.config.js  # Site configuration
```

## Local Development

Start your site locally:

```bash
npm install
npm start
```

Your site will be available at `http://localhost:3000`.

## Building for Production

Build your site for production:

```bash
npm run build
```

This generates static content into the `build` directory which can be served by any static hosting service, including QuantCDN.

## Deployment

This template includes a GitHub Actions workflow that automatically deploys your site to QuantCDN when you push to the main branch.

### Required Secrets

Configure these secrets in your GitHub repository:

- `QUANT_CUSTOMER` - Your QuantCDN customer ID
- `QUANT_PROJECT` - Your QuantCDN project name
- `QUANT_TOKEN` - Your QuantCDN API token

## Learn More

- [Docusaurus Documentation](https://docusaurus.io/docs)
- [QuantCDN Documentation](https://docs.quantcdn.io/)
