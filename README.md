# stylesheet-cdn

A collection of CSS stylesheets served via free CDN for easy integration into your projects.

## Available Stylesheets

- `github-markdown.css` - GitHub-flavored Markdown styling with white background
- `dhdhagar.vscode-md-preview-light.css` - VS Code Markdown Preview Light theme
- `mahonnaise.vs-code-markdown-theme.css` - VS Code Markdown theme

## Usage

### jsDelivr CDN (Recommended)

Include any stylesheet in your HTML:

```html
<!-- GitHub Markdown styling -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/Gekyzo/stylesheet-cdn@main/styles/github-markdown.css">

<!-- VS Code Markdown Preview Light -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/Gekyzo/stylesheet-cdn@main/styles/dhdhagar.vscode-md-preview-light.css">

<!-- VS Code Markdown theme -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/Gekyzo/stylesheet-cdn@main/styles/mahonnaise.vs-code-markdown-theme.css">
```

### Version-specific URLs

For production use, it's recommended to use tagged versions:

```html
<!-- Replace v1.0.0 with the specific version you want -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/Gekyzo/stylesheet-cdn@v1.0.0/styles/github-markdown.css">
```

## How It Works

This repository uses [jsDelivr](https://www.jsdelivr.com/) to serve files directly from GitHub. jsDelivr automatically provides:

- Fast global CDN delivery
- Automatic minification (add `.min` before file extension)
- Version control via Git tags
- No signup or configuration required

## Adding New Stylesheets

1. Add your CSS file to the `styles/` folder
2. Commit and push to GitHub
3. Access via: `https://cdn.jsdelivr.net/gh/Gekyzo/stylesheet-cdn@main/styles/your-file.css`

## Notes

- Files are cached by the CDN, so changes may take 5-10 minutes to propagate
- Always use version tags for production to ensure stability
- Repository must remain public for CDN access to work