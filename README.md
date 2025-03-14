# Figma CSS Variables Plugin

> [!NOTE]
> This repository hosts the [Github Discussion community](https://github.com/figma-css-variables/community/discussions) for the [Figma CSS Variables plugin](https://www.figma.com/community/plugin/1474166340745390696/figma-css-variables).<br />
> Check the [FAQ](FAQ.md) or [GitHub Discussions](https://github.com/figma-css-variables/community/discussions) for support.

Effortlessly export your Figma variables to CSS. Git deployment is coming soon!

[![Image of Figma CSS Variables plugin](https://yoriiis.github.io/cdn/static/figma-css-variables/cover-1.png)](https://www.figma.com/community/plugin/1474166340745390696/figma-css-variables)

## Features

### Export & Sync

- **Analyze your variables** View all Figma variable collections and modes
- **Instant CSS generation** Preview and export CSS from your variables
- **Flexible export options** Copy CSS directly or download all generated CSS files
- **One-click synchronization** Always stay up to date with your latest Figma variables
- When exporting, a **ZIP file** is generated with all the CSS files at the root level

### Deploy to Git (coming soon)

A powerful **Git deployment** feature is coming soon! This will allow you to automatically deploy your generated **CSS variable files** to **Git** for seamless design–code collaboration.

We'd love to hear your thoughts and feedback on this upcoming feature! Feel free to join the discussion on [GitHub Discussions](https://github.com/figma-css-variables/community/discussions).

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
- Copy the generated CSS directly to your clipboard or download all CSS files

---

Made with ❤️ by [@yoriiis](https://github.com/yoriiis)
