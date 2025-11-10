# Deployment Guide for GitHub Pages

## Initial Setup

1. **Create GitHub Repository**
   ```bash
   # Initialize git (if not already done)
   git init
   
   # Add all files
   git add .
   
   # Commit
   git commit -m "Initial commit: Multi-restaurant POS system"
   
   # Add remote (replace with your repository URL)
   git remote add origin https://github.com/nagasakimark/cashregister2.git
   
   # Push to GitHub
   git push -u origin main
   ```

2. **Enable GitHub Pages**
   - Go to your repository on GitHub
   - Click "Settings"
   - Scroll to "Pages" section
   - Under "Source", select "main" branch
   - Click "Save"
   - Your site will be available at: `https://nagasakimark.github.io/cashregister2/`

## Updating the Site

After making changes:

```bash
git add .
git commit -m "Description of changes"
git push
```

GitHub Pages will automatically rebuild and deploy your changes within a few minutes.

## Notes

- The `.gitignore` file excludes development files and documentation
- Only production-ready files are deployed
- Images and fonts are included for the live site
- Menu configurations are loaded dynamically from JSON files
