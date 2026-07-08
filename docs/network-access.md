# Design Tokens Export & Deploy: Network Access

> [!IMPORTANT]
> This document outlines the network resources the plugin (Figma and Penpot versions) connects to.

In this document, "platform" refers to Figma or Penpot depending on which version you use.

## All users

### Sentry

We use **Sentry** to track errors and crashes, helping us identify and resolve issues efficiently.

Error reports include a hashed user identifier (SHA-256, one-way and irreversible) and context such as the error type and subscription plan. No personally identifiable information (PII) is sent.

### PostHog

We use **PostHog** to collect anonymous usage analytics.

Collected data is limited to feature usage, plugin version, and platform type. No personally identifiable information (PII) or design content is sent.

### Git Providers

When users use the **Git provider** feature, the plugin connects directly to the GitHub API, GitLab API (including self-hosted instances), Bitbucket API or Azure DevOps API to deploy the exported design token files.

Connections occur directly between the plugin and the chosen provider. No data passes through our infrastructure.

### Subscription status

The plugin periodically checks your subscription status to determine which features are available. This sends your platform user ID and platform name to our API.

Payments are processed by **Stripe**. No payment data passes through our infrastructure.

## Data storage

- **User ID** is stored on the backend (encrypted at rest) for subscription management
- **Subscription status** is cached locally with cryptographic signature verification
- Git provider credentials (tokens) are stored locally using the platform's official storage API and never sent to our servers

## Security

For details on reporting vulnerabilities, see [SECURITY.md](../.github/SECURITY.md).
