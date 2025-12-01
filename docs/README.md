# TikSpyder GitHub Pages

This directory contains the static website for TikSpyder that is published to GitHub Pages.

## About

TikSpyder is a Python-based Streamlit application that cannot run directly on GitHub Pages (which only supports static content). This GitHub Pages site serves as:

- A landing page with project information
- Installation and usage instructions
- Links to the GitHub repository
- Examples and documentation

## Local Development

To preview the site locally:

1. Open `index.html` in a web browser
2. Or use a simple HTTP server:
   ```bash
   python -m http.server 8000
   ```
   Then visit http://localhost:8000

## Deployment

The site is automatically published to GitHub Pages when changes are pushed to the main branch.

**GitHub Pages Settings:**
- Source: Deploy from a branch
- Branch: main (or your default branch)
- Folder: /docs

## Running the Actual Application

To run the TikSpyder Streamlit application:

1. Clone the repository
2. Install dependencies: `pip install -r requirements.txt`
3. Launch: `tikspyder --app` or `streamlit run app.py`

For full documentation, see the main [README.md](../README.md) in the repository root.
