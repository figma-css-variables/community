# Frequently Asked Questions (FAQ) - Figma CSS Variables

Welcome to the FAQ for Figma CSS Variables. Here you'll find answers to common questions to help you get started and troubleshoot issues efficiently.

## 🚀 Getting started

<details>

<summary>How do I install the Figma CSS Variables plugin?</summary>

<br />

Go to the [plugin page on Figma Community](https://www.figma.com/community/plugin/1474166340745390696/figma-css-variables) and click "Open in...". Then open a Figma file, go to Plugins > Figma CSS Variables.
See [Use plugins in files from Figma resource](https://help.figma.com/hc/en-us/articles/360042532714-Use-plugins-in-files).

</details>

<details>

<summary>The plugin won't launch, what should I do?</summary>

<br />

Ensure Figma is up to date and that the plugin is properly installed. Check your internet connection and look for any errors displayed in Figma. Additionally, try restarting both Figma and the plugin.

Check the browser's Developer Tools (right-click > Inspect > Console tab). If there are errors, share them on the [GitHub Discussions](https://github.com/figma-css-variables/community/discussions) with a reproduction scenario and captures of the error messages.

</details>

## 💳 Subscription

<details>

<summary>How do I subscribe?</summary>

<br />

Click the **Subscribe** button in the plugin (visible on the Deploy or Export tab when you're not subscribed). You'll be redirected to Stripe Checkout to complete the payment. After a successful payment, your access is updated automatically.

</details>

<details>

<summary>How do I manage or cancel my subscription?</summary>

<br />

Go to the **Settings** tab and click **Manage subscription**. You'll be redirected to Stripe Customer Portal where you can update your payment method, view invoices, or cancel your subscription.

</details>

<details>

<summary>What happens if my payment fails?</summary>

<br />

Stripe will retry the payment automatically. If the payment continues to fail, your subscription will be marked as inactive and Pro features will be locked. You can update your payment method through the Stripe Customer Portal (Settings > Manage subscription).

</details>

<details>

<summary>What features are included in the subscription?</summary>

<br />

See the [Pro section in the README](README.md#pro) for the full list of features included with a subscription.

The **Export tab** (preview and copy to clipboard) remains free for all users.

</details>

<details>

<summary>Is my subscription tied to a specific Figma account?</summary>

<br />

Yes. Your subscription is linked to the **Figma account** you used when subscribing. Make sure you're logged into the same Figma account when using the plugin. If you use multiple Figma accounts, you'll need a subscription for each one.

</details>

## 🔑 Existing license holders

<details>

<summary>I had a license before. What do I need to do?</summary>

<br />

Nothing. Your license was automatically linked to your Figma account. If your Pro status doesn't show as active, go to **Settings > Refresh** to force a status check.

</details>

## ⚙️ Usage

<details>

<summary>How do I export my CSS variables?</summary>

<br />

Go to the Export tab, select a collection and mode, preview the CSS, then copy it to your clipboard. **Pro users**: download all files as a ZIP.

</details>

<details>

<summary>Some variables aren't exporting properly. What's happening?</summary>

<br />

The plugin applies transformations to ensure CSS validity:

- Slashes (/) are replaced with hyphens (-).
- Numeric variables (FLOAT) automatically append the px unit.
- CSS variables are sorted alphabetically.

</details>

<details>

<summary>Can I export multiple collections at once?</summary>

<br />

The **Download all** option (Pro) exports all selected collections at once in a ZIP file. For the copy-to-clipboard option, only one mode of a collection is copied. The **Git deployment** feature (Pro) also lets you select specific collections and modes to deploy.

</details>

## 🌐 Git Deployment (Pro)

<details>

<summary>How do I enable Git deployment?</summary>

<br />

First, subscribe via the plugin (click Subscribe on the Deploy or Export tab). Once subscribed, go to the **Settings** tab to add a Git provider. Then go to the **Deploy** tab, select your provider, choose the collection modes to export, and click the **Push** button.

If the subscription status doesn't update immediately, click the **Refresh** button in the Settings tab.

</details>

<details>

<summary>I can't add a Git provider. What should I check?</summary>

<br />

Ensure your personal access token is valid and has the necessary permissions and the user/organization name, repository and branch are correct. For self-hosted GitLab, include the host URL `mycustomgitlab.com`.

Check resources:

- [Github Personal Access Token documentation](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-token)
- [Gitlab Personal Access Token documentation](https://docs.gitlab.com/user/profile/personal_access_tokens)

</details>

<details>

<summary>My push to Git fails. How can I fix it?</summary>

<br />
Troubleshoot with these steps:

- Check that the token has sufficient write permissions
- Verify the branch exists (the plugin will create it automatically if permissions allow)
- Ensure the repository URL and provider details are correct
- Confirm that the selected collections and modes are not empty

</details>

<details>

<summary>Can I push to specific branches?</summary>

<br />

Yes, you can specify the target branch in the provider settings. If the branch doesn't exist, the plugin will create it automatically.

</details>

<details>

<summary>Can I push to specific directories?</summary>

<br />

Yes, you can specify the base path in the provider settings. If the directories don't exist, the plugin will create it automatically.

</details>

## 🔐 Security

<details>

<summary>Where are my Git provider details stored?</summary>

<br />

All Git provider data (token, owner, repository, etc.) is stored locally on your machine to ensure your privacy and security.

</details>

<details>

<summary>What data does the plugin send to your servers?</summary>

<br />

When checking subscription status, the plugin sends your **Figma User ID** to verify your access. No email or personal information is sent.

</details>

## Troubleshooting

<details>

<summary>I subscribed but the plugin still shows Inactive. What should I do?</summary>

<br />

First, make sure you're logged into the same **Figma account** used for the subscription. Then go to the **Settings** tab and click the **Refresh** button to force a status check. If it still shows Inactive, try closing and reopening the plugin.

Activation is automatic and usually takes a few seconds. The Refresh button simply speeds up the process.

</details>

<details>

<summary>The deployment fails every time. What can I check?</summary>

<br />

Make sure:

- The token has the necessary permissions
- The target branch exists or that your token allows branch creation
- The selected collections and modes aren't empty

</details>

## 📬 Contact & Support

<details>

<summary>How do I report a bug or request a feature?</summary>

<br />

Use the [GitHub Issues](https://github.com/figma-css-variables/community/issues) page for bug reports or feature requests. For general questions, join the [GitHub Discussions](https://github.com/figma-css-variables/community/discussions).

</details>

<details>

<summary>How can I get support?</summary>

<br />

If your question isn't covered here, please post in our [GitHub Discussions](https://github.com/figma-css-variables/community/discussions), and we'll help as soon as possible.

</details>
