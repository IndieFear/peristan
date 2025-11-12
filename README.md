# peristan

Personal portfolio website built with Hugo and the Hextra theme.

## Local Development

```bash
# Install dependencies
hugo mod download

# Start development server
hugo server --buildDrafts --disableFastRender
```

## Deployment to GitHub Pages

This site is automatically deployed to GitHub Pages using GitHub Actions.

### Setup Instructions

1. **Create a GitHub repository** (if not already created)
   ```bash
   git remote add origin https://github.com/IndieFear/peristan.git
   ```

2. **Push your code to GitHub**
   ```bash
   git add .
   git commit -m "Initial commit"
   git push -u origin main
   ```

3. **Enable GitHub Pages**
   - Go to your repository on GitHub
   - Navigate to **Settings** → **Pages**
   - Under **Source**, select **GitHub Actions**
   - The workflow will automatically deploy on every push to `main`

4. **Update baseURL** (if needed)
   - If your repository is named `peristan`, your site will be available at `https://IndieFear.github.io/peristan/`
   - Update `baseURL` in `hugo.yaml` accordingly, or use the default GitHub Pages URL

### Custom Domain (Optional)

If you want to use `peristan.co`:
1. Add a `CNAME` file in the `static/` directory with your domain
2. Configure DNS records as per GitHub Pages documentation
3. Update `baseURL` in `hugo.yaml` to your custom domain

## Project Structure

```
peristan/
├── content/          # Site content (Markdown files)
├── static/          # Static files (images, etc.)
├── hugo.yaml       # Hugo configuration
├── go.mod          # Hugo Modules dependencies
└── .github/        # GitHub Actions workflows
```

