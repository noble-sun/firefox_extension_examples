# Firefox WebExtension Examples

This repository contains two beginner-friendly Firefox WebExtension examples from the Mozilla Developer Network (MDN). These examples demonstrate key concepts like content scripts, browser actions, popup UIs, and inter-script messaging.

## 📁 Contents

### 1. `borderify/` – Your First WebExtension

**Tutorial**: [Your first extension](https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/WebExtensions/Your_first_WebExtension)

**Description**:  
This extension applies a red border to all web pages on `mozilla.org`. It demonstrates how to:

- Inject a content script into pages.
- Use the `manifest.json` file to declare resources and permissions.
- Match specific websites using URL patterns.

**Key Files**:
- `manifest.json` – Describes the extension's metadata and behavior.
- `borderify.js` – A content script that modifies the page's CSS.

---

### 2. `beastify/` – Your Second WebExtension

**Tutorial**: [Your second extension](https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/WebExtensions/Your_second_WebExtension)

**Description**:  
This extension adds a browser toolbar button. When clicked, a popup appears allowing the user to "beastify" the current page — replacing its content with an image of a beast (e.g., frog, snake, turtle). It demonstrates:

- Creating and styling a popup.
- Sending messages from the popup to a content script.
- Injecting scripts on demand.

**Key Files**:
- `manifest.json` – Declares the extension’s popup and content scripts.
- `popup.html`, `popup.js` – The UI and logic for the popup window.
- `beastify.js` – The content script that alters the webpage.
- `remove.js` – A script to reset the page.
- `images/` – Web-accessible images used in the popup.

---

## 🚀 How to Run These Extensions

1. Clone the repository with:
```bash
git clone git@github.com:noble-sun/firefox_extension_examples.git
```
2. Open Firefox and go to `about:debugging`.
3. Click **"This Firefox"**.
4. Click **"Load Temporary Add-on..."**.
5. Select the `manifest.json` file from the `borderify` or `beastify` directory.

The extension will now be active for your current Firefox session.

---

## 🛠 Requirements

- Firefox 48 or later.
- No build tools required — just plain HTML, JS, and JSON.

---

## 📄 License

These examples are derived from publicly available MDN documentation and are intended for educational purposes. For original content and license information, refer to Mozilla's [Terms of Use](https://www.mozilla.org/en-US/about/legal/).

---

## 🙏 Acknowledgments

- [MDN Web Docs – WebExtensions](https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/WebExtensions)

