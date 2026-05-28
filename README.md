# Figma CSS Variables Plugin

> [!NOTE]
> This repository hosts the [Github Discussion community](https://github.com/figma-css-variables/community/discussions) for the [Figma CSS Variables plugin](https://www.figma.com/community/plugin/1474166340745390696/figma-css-variables).<br />
> Check the [FAQ](FAQ.md) or [GitHub Discussions](https://github.com/figma-css-variables/community/discussions) for support.

Export your Figma variables to CSS and deploy them to Git.

[![Image of Figma CSS Variables plugin](https://yoriiis.github.io/cdn/static/figma-css-variables/cover-1.png)](https://www.figma.com/community/plugin/1474166340745390696/figma-css-variables)

## Features

### Free

- **Analyze your variables** View all Figma variable collections and modes
- **Instant CSS generation** Preview and export CSS from your variables
- **Copy to clipboard** Copy the generated CSS for a single mode
- **One-click synchronization** Always stay up to date with your latest Figma variables

### Pro

Everything in **Free**, plus:

- **Download all** Export all collections and modes as a ZIP file
- **Git deployment** Push your CSS files directly to GitHub, GitLab, or self-hosted GitLab
- Select specific collections and modes to deploy
- Commit messages are automatically generated

Subscriptions are managed through Stripe directly from the plugin.

### File structure

- A separate **CSS file** is generated for each mode within a collection
- Files follow the naming pattern: "collectionName-modeName.css"

### Variable transformations

Figma variables are transformed to ensure they are valid in **CSS**:

- Slashes (`/`) are replaced with hyphens (`-`) in variable names
- Original casing of variable names is preserved (uppercase, lowercase, etc.)
- For numeric variables (`FLOAT` type), the unit `px` is automatically added
- CSS variables are sorted alphabetically

### UI & Accessibility

- **Dark mode compatible**: the plugin adapts to the user's Figma theme preference (light/dark mode)
- **Keyboard navigation**: all interactive elements support keyboard navigation for improved accessibility
- **Focus indicators**: clear visual focus on form fields and interactive elements
- **Accessibility compliance**: designed following W3C and A11Y best practices

## How to use

### Exporting CSS Variables

- Navigate to the **Export** tab
- View all Figma variables structured into **collections** and **modes** (a collection contains multiple modes)
- Select a collection and a mode
- Preview the generated CSS
- Copy the generated CSS directly to your clipboard
- **Pro users**: download all files as a ZIP

### Deploying to Git

- Navigate to the **Settings** tab and add a Git provider
- Go to the **Deploy** tab
- Select your provider, choose the collections and modes to export
- Click the **Push** button to deploy

---

Made with ❤️ by [@yoriiis](https://github.com/yoriiis)
