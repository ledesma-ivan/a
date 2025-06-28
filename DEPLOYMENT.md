# GitHub Pages Deployment Guide

## 🚀 Quick Setup

Your site is now ready for GitHub Pages deployment! Follow these steps:

### 1. Push to GitHub

```bash
git add .
git commit -m "Add GitHub Pages configuration"
git push origin main
```

### 2. Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on **Settings** tab
3. Scroll down to **Pages** section (in the left sidebar)
4. Under **Source**, select **Deploy from a branch**
5. Choose **main** branch and **/docs** folder
6. Click **Save**

### 3. Configure GitHub Actions (Optional)

The GitHub Actions workflow will automatically deploy your site when you push changes. To enable it:

1. Go to **Settings** → **Pages**
2. Under **Build and deployment**, select **GitHub Actions** as the source
3. The workflow will run automatically on the next push

### 4. Custom Domain (Optional)

If you have a custom domain:

1. Add your domain to the `docs/CNAME` file
2. Go to **Settings** → **Pages**
3. Enter your custom domain in the **Custom domain** field
4. Save the changes

## 📝 Important Notes

- The site is already built and ready in the `docs/` folder
- The `.nojekyll` file ensures GitHub Pages serves the static files correctly
- Your site will be available at: `https://yourusername.github.io/repository-name`

## 🔧 Troubleshooting

- **404 errors**: Make sure all links in your HTML files are relative (start with `/`)
- **Styling issues**: Check that all CSS and assets are properly linked
- **Build failures**: Check the Actions tab for detailed error messages

## 📞 Support

If you encounter any issues, check the [GitHub Pages documentation](https://docs.github.com/en/pages) or create an issue in this repository. 