# Figma CSS Variables Plugin

> This repository hosts the [Github Discussion community](https://github.com/figma-css-variables/community/discussions) for the [Figma CSS Variables plugin](https://www.figma.com/community/plugin/1474166340745390696/figma-css-variables).

Effortlessly export your Figma variables to CSS and deploy them to Git.

[![Image of Figma CSS Variables plugin](https://yoriiis.github.io/cdn/static/figma-css-variables/cover-1.png)](https://www.figma.com/community/plugin/1474166340745390696/figma-css-variables)

## Features

### Export & Sync

- **Analyze your variables** View all Figma variable collections and modes
- **Instant CSS generation** Preview and export CSS from your variables
- **Flexible export options** Copy CSS directly or download all generated CSS files
- **One-click synchronization** Always stay up to date with your latest Figma variables
- When exporting, a **ZIP file** is generated with all the CSS files at the root level

### Deploy to Git (Premium feature)

This feature allows you to automatically deploy your generated **CSS variable files** to **Git** for seamless design–code collaboration.

Unlock **Git deployment** by purchasing directly through **Figma**. No third-party payment is required.

- Connect to **GitHub**, **GitLab**, or a **self-hosted GitLab** instance
- Select multiple **collections & modes** to deploy in a single commit
- **Commit messages** are automatically pre-filled based on your selection
- **Branches** are customizable and automatically created if they do not exist
- Customize the **target directory** for your CSS files using the `basePath` parameter
- Simplify collaboration between **design** and **development**

### Git Integration & Security

You can easily manage your **Git providers** by:

- **Adding** a new provider
- **Editing** the settings of an existing provider
- **Deleting** a provider if it's no longer needed

When saving a Git provider, the following fields are available:\
`token`, `owner`, `repository`, `branch`, `basePath` and `host` (for self-hosted GitLab).

Your Git provider details are **stored locally** on your machine for **privacy** and **security**.

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

### Deploying to Git (Premium feature)

- First, add a Git provider from the **Settings** tab
- Choose a provider from the available options (**GitHub**, **GitLab**)
- Fill in the required details in the configuration modal
- Save the provider settings
- Next, go to the **Deploy** tab and select a provider from the list
- Use the **multiple selection dropdown** to choose the **modes** you wish to deploy
- Click **Push** to deploy the corresponding CSS files to Git

---

Made with ❤️ by [@yoriiis](https://github.com/yoriiis)
