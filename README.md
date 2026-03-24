# Amanitaceae.org Backup

Complete backup of http://amanitaceae.org formatted for GitHub Pages.

## What's Included

- **22MB** of data across **244 files**
- **204 HTML pages** covering Amanita species, taxonomy, news, and research
- Images, CSS, JavaScript, and PDF documents
- All links converted to be relative for GitHub Pages deployment

## Deployment to GitHub Pages

The site is ready for GitHub Pages deployment. Follow these steps:

### Option 1: Manual Setup (Recommended)
1. Go to your repository on GitHub
2. Click **Settings** > **Pages**
3. Under **Build and deployment** > **Source**, select **Deploy from a branch**
4. Under **Branch**, select **main** and folder **/docs**
5. Click **Save**
6. Wait a few minutes for deployment to complete
7. Your site will be available at: `https://[your-username].github.io/amanitaceae-org-backup/`

### Option 2: Automatic via GitHub Actions
The repository includes a GitHub Actions workflow (`.github/workflows/deploy.yml`) that will automatically deploy to GitHub Pages when you push to the main branch.

## Site Structure

- `docs/index.html` - Redirects to the main Home page
- `docs/Home.html` - Main homepage
- `docs/Amanita_*.html` - Individual Amanita species pages
- `docs/site_news_*.html` - News articles from 2010-2022
- `docs/image/` - All images from the original site
- `docs/scripts/` - JavaScript files (including xajax framework)
- `docs/template/` - CSS and font files

## Important Notes

1. **Static Snapshot**: The original site uses PHP and the xajax AJAX framework for dynamic content loading. This backup contains static HTML snapshots of each page as it appeared when downloaded.

2. **Limited Interactivity**: Some interactive features that relied on PHP/xajax won't work in this static version, but all content is preserved.

3. **Navigation**: All internal links have been fixed to work with the renamed HTML files and relative paths.

4. **External Links**: Links to external resources (other websites, etc.) remain intact.

## Technical Details

- Downloaded using `wget --mirror --convert-links --adjust-extension --page-requisites`
- Query parameter URLs converted to proper filenames (e.g., `?Amanita muscaria` → `Amanita_muscaria.html`)
- All internal links updated to use relative paths
- Organized in `/docs` directory for GitHub Pages compatibility

## License

This is a backup of content from http://amanitaceae.org. All original content copyright belongs to the respective authors and the Amanitaceae.org website.
