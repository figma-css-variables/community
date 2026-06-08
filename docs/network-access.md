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

### Subscription status

The plugin periodically checks your subscription status to determine which features are available.

Payments are processed by **Stripe**. No payment data passes through our infrastructure.
