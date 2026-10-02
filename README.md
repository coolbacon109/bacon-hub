# ❄️ Arctic & LazyList Secure Portal

A highly stealthy, password-protected web portal designed to securely deploy massive standalone HTML payloads. Built with a premium "liquid glass" aesthetic, this portal uses advanced browser-level cloaking to ensure sessions remain hidden, untracked, and completely detached from the host domain.

Made with love by coolbacon <3

## ✨ Features

*   **🔒 Multi-User Authentication:** Secure gateway requiring a predefined passcode to access the portal payloads.
*   **💧 Liquid Glass UI:** A responsive, ultra-clean frosted glass interface with ambient fluid background blobs and custom cubic-bezier pop-in animations.
*   **👻 Advanced Tab Cloaking:** Instantly disguises the portal as an educational utility (e.g., Clever, Canvas) by manipulating the document title and favicon.
*   **🛡️ `about:blank` Injection:** Launches payloads directly into a detached, borderless `about:blank` window via hidden iframes. This bypasses standard history tracking and prevents massive CSS/JS files from conflicting with the main portal.
*   **⚡ Zero-Trace Redirection:** Instantly covers its tracks by auto-redirecting the original host tab to a safe website (Google or Clever) the millisecond a payload is launched.
*   **📥 Direct Local Downloads:** Allows users to bypass browser restrictions entirely by downloading the massive HTML payloads directly to their local machine.

## 🚀 Deployment (GitHub Pages)

To host this securely on GitHub Pages:

1.  Upload `index.html` to the root of your repository.
2.  Upload your payload files directly next to `index.html`. They **must** be named exactly:
    *   `lazylist.html`
    *   `arctic.html`
3.  Upload your rejection screen audio as `audio.mp3`.
4.  Go to **Settings** > **Pages**.
5.  Under **Build and deployment**, set the Source to **Deploy from a branch**.
6.  Select your `main` branch and click **Save**. 

*Note: It may take up to 2 minutes for GitHub to build and deploy your live site.*

## ⚙️ Configuration

To change the access codes or add new users, modify the `ALLOWED_PASSCODES` array located in the script section of `index.html`:

```javascript
const ALLOWED_PASSCODES = ["coolbacon", "luisisthebest", "nosery", "kingsley", "masonmason"];
