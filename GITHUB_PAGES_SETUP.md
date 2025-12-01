# GitHub Pages Deployment Guide

## Quick Setup Instructions

To enable GitHub Pages for this repository, follow these steps:

### 1. Navigate to Repository Settings
1. Go to your GitHub repository: https://github.com/extremerom/tik-spyder
2. Click on **Settings** tab (near the top right)
3. In the left sidebar, scroll down and click on **Pages**

### 2. Configure GitHub Pages Source
In the "Build and deployment" section:

- **Source**: Select `Deploy from a branch`
- **Branch**: Select your default branch (usually `main` or `master`)
- **Folder**: Select `/docs`
- Click **Save**

### 3. Wait for Deployment
- GitHub will automatically build and deploy your site
- This typically takes 1-5 minutes
- You'll see a green checkmark when deployment is complete

### 4. Access Your Site
Your site will be available at:
```
https://extremerom.github.io/tik-spyder/
```

### 5. Verify Deployment
After a few minutes:
1. Visit the URL above
2. You should see the TikSpyder landing page
3. If you see a 404 error, wait a bit longer and refresh

## What Was Created

The following files were added to enable GitHub Pages:

```
docs/
├── index.html       # Main landing page
├── styles.css       # CSS styling (TikTok-inspired dark theme)
├── _config.yml      # GitHub Pages configuration
├── .nojekyll        # Prevents Jekyll processing
└── README.md        # Documentation for the docs folder
```

## Features of the Landing Page

✨ **Professional Design**
- TikTok-inspired dark theme
- Fully responsive (mobile, tablet, desktop)
- Smooth animations and transitions
- Modern, clean interface

📱 **Comprehensive Content**
- Project overview and description
- Key features showcase
- Installation instructions
- Usage examples (CLI and Web UI)
- Requirements and dependencies
- Support links

🎨 **Optimized for GitHub Pages**
- Static HTML/CSS (no build process needed)
- Fast loading
- SEO-friendly meta tags
- Works without JavaScript (enhanced with JS)

## Customization

### Updating Content
To update the landing page content:
1. Edit `docs/index.html`
2. Commit and push changes
3. GitHub Pages will automatically redeploy (within minutes)

### Updating Styles
To modify the appearance:
1. Edit `docs/styles.css`
2. Commit and push changes
3. Changes will appear after redeployment

### Color Scheme
The current theme uses TikTok-inspired colors:
- Primary Accent: `#fe2c55` (TikTok Red/Pink)
- Secondary Accent: `#25f4ee` (TikTok Cyan)
- Background: `#0e1117` (Dark)
- Cards: `#262730` (Dark Gray)

## Troubleshooting

### 404 Error
- **Problem**: Site shows "404 - Page Not Found"
- **Solution**: 
  - Ensure `/docs` folder is selected in settings
  - Wait 5-10 minutes for initial deployment
  - Check that `index.html` exists in `/docs` folder
  - Verify the branch selected in settings has the `/docs` folder

### Styles Not Loading
- **Problem**: Page appears but without styling
- **Solution**:
  - Check that `styles.css` is in the same folder as `index.html`
  - Verify the link tag in `index.html` references `styles.css` (not `/styles.css`)
  - Clear browser cache and refresh

### Changes Not Appearing
- **Problem**: Updates to files don't show on the site
- **Solution**:
  - Wait 2-5 minutes for GitHub Pages to rebuild
  - Check the "Actions" tab for deployment status
  - Clear browser cache (Ctrl+Shift+R or Cmd+Shift+R)

## Important Notes

⚠️ **Streamlit App Limitation**
The main TikSpyder application is a Streamlit app that **cannot run directly on GitHub Pages** because:
- GitHub Pages only serves static content (HTML, CSS, JS)
- Streamlit requires a Python server to run
- The landing page serves as documentation and installation guide

🚀 **Running the Actual App**
Users must:
1. Clone the repository
2. Install dependencies: `pip install -r requirements.txt`
3. Run locally: `tikspyder --app` or `streamlit run app.py`

Or deploy to:
- [Streamlit Cloud](https://streamlit.io/cloud) (recommended)
- [Heroku](https://www.heroku.com/)
- [Railway](https://railway.app/)
- Any cloud platform supporting Python apps

## Next Steps

After enabling GitHub Pages:

1. ✅ Verify the site is accessible
2. ✅ Share the GitHub Pages URL in your README (already done)
3. ✅ Consider adding the URL to repository description
4. ✅ Update social media with the new landing page link
5. 📝 Monitor GitHub Pages deployment in the Actions tab

## Additional Resources

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Custom Domain Setup](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)
- [HTTPS on GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/securing-your-github-pages-site-with-https)

---

**Questions or Issues?**
If you encounter any problems, please open an issue on the repository.
