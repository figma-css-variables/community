# Figma CSS Variables: Network Access

> [!IMPORTANT]
> This document outlines the network resources the Figma plugin connects to when using the Community build.

The Figma plugin interacts with specific services to ensure proper functionality while maintaining user privacy and security.

## All users

### Sentry

We use **Sentry** to track errors and crashes, helping us identify and resolve issues efficiently.

The plugin sends error reports to `sentry.io`. These reports do not contain any personally identifiable information (PII).

### Git Providers

When users utilize the **Git provider** feature, the plugin connects directly to GitHub, GitLab, or a self-hosted GitLab instance to deploy CSS files.

Connections occur directly between the plugin and the user's chosen provider; no data passes through our infrastructure. All data is stored locally within the Figma application.

## Licensed Users

### License validation

The **Git deployment** feature requires a valid license, which is verified through a Netlify Edge Function hosted at `figmacssvariables-api.netlify.app`. This process checks the license key and Figma User ID to ensure authorized usage.

License data is stored on **Supabase**, while payments are processed via **Stripe**. The email associated with the Stripe subscription is used to link a license to a user.

No unnecessary personal data is collected, and all information is handled securely.
