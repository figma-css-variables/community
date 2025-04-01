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

## 🔑 License management

<details>

<summary>I didn't receive my license after purchase. What should I do?</summary>

<br />

Check your spam folder. Emails are sent from the email address `figmacssvariables[at]yoriiis.com`. If you still can't find the email, reach out to us with your proof of purchase, and we'll generate a new license for you.

</details>

<details>

<summary>My license doesn't work. What should I check?</summary>

<br />

Ensure you copied the license correctly without any extra spaces. The license is tied to the email used during purchase.

Ensure you copied the license correctly without any extra spaces. The license is tied to the email used during purchase. The format of a valid license key looks like this: `XXXXXX-XXXXXX-XXXXXX-XXXXXX-XXXXXX-V1`, where each `X` is a random alphanumeric character.

</details>

<details>

<summary>What if I lose my license?</summary>

<br />

For security reasons, licenses are not stored in plain text. If you lose your license, contact us at `figmacssvariables[at]yoriiis.com` to generate a new one.

</details>

<details>

<summary>My license is expired. What should I do?</summary>

<br />

If your subscription has been canceled or the payment has failed, and the validity period has expired, the license becomes inactive. To reactivate your license, ensure your subscription is active on Stripe. If needed, renew it directly through Stripe or contact support at `figmacssvariables[at]yoriiis.com` with your proof of purchase. Once the subscription is active again, the license will be restored automatically.

</details>

## ⚙️ Usage

<details>

<summary>How do I export my CSS variables?</summary>

<br />

Go to the Export tab, select a collection and mode, preview the CSS, then either copy it to your clipboard or download a ZIP containing all the CSS files.

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

For the download option, all selected collections are exported at once in a ZIP file. For the copy-to-clipboard option, only one mode of a collection is copied. To export multiple modes or collections, use the Git Deployment feature to choose specific collections and modes.

</details>

## 🌐 Git Deployment (Premium)

<details>

<summary>How do I enable Git deployment?</summary>

<br />

First, purchase a license directly through Figma and activate it in the plugin's Settings tab. Then, create a Git provider under the Settings tab. After that, go to the Deploy tab, select your provider from the list, choose the collection modes to export, and click the "Push" button to deploy.

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
  Verify the branch exists (the plugin will create it automatically if permissions allow)
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

Yes, you can specify the base path in the provider settings. If the directories doesn't exist, the plugin will create it automatically.

</details>

## 🔐 Security

<details>

<summary>Where are my Git provider details stored?</summary>

<br />

All Git provider data (token, owner, repository, etc.) is stored locally on your machine to ensure your privacy and security.

</details>

<details>

<summary>Can I share my license with others?</summary>

<br />

No, each license is personal and linked to the email used during purchase.

</details>

## Troubleshooting

<details>

<summary>I'm getting an `License is expired or inactive` error. What should I do?</summary>

<br />

Double-check the license key you entered, ensuring there are no extra spaces or typos. Check if the susbcription is active on Stripe. If the issue persists, contact support at `yoriiis[at]duck.com`.

</details>

<details>

<summary>The deployment fails every time. What can I check?</summary>

<br />

Make sure:

The token has the necessary permissions.

The target branch exists or that your token allows branch creation.

The selected collections and modes aren't empty.

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
