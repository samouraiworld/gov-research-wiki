# Obsidian Notes with Quartz

This repository publishes Obsidian notes as a static website using [Quartz](https://quartz.jzhao.xyz/).

## Structure

- `sources/` - Your Obsidian notes (this is your vault content)
- `quartz.config.ts` - Quartz configuration
- `quartz.layout.ts` - Layout configuration
- `public/` - Generated static site (git-ignored)

## Local Development

1. Install dependencies:
   ```bash
   npm install
   ```

2. Build the site:
   ```bash
   npx quartz build --directory sources
   ```

3. Serve locally with live reload:
   ```bash
   npx quartz build --serve --directory sources
   ```

## Deployment

The site automatically deploys to GitHub Pages when you push to the `main` branch. The GitHub Action workflow builds and deploys your notes.

Your site will be available at: `https://samouraiworld.github.io/gov-research-wiki/`

## Adding Notes

Simply add or edit Markdown files in the `sources/` directory. The Quartz build process will automatically:

- Parse Obsidian-flavored Markdown
- Convert wikilinks (`[[note]]`) to proper links
- Generate a searchable site with navigation
- Apply syntax highlighting and LaTeX rendering

## Configuration

Edit `quartz.config.ts` to customize:
- Site title and metadata
- Theme colors and fonts
- Plugins and features
- Analytics and SEO settings
