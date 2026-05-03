# Grumpy AI Rescue Engine - Browser CDN SDK

This is the vanilla JavaScript SDK for the Grumpy AI Rescue Engine. It is designed to be included directly in HTML templates (Jinja2, Django, Laravel, Blade, or static HTML) via a `<script>` tag.

## Features
- **Global Error Handling:** Hooks into `window.onerror` and `window.unhandledrejection`.
- **Zero Dependencies:** Pure vanilla JavaScript.
- **Rescue Engine Compatible:** Automatically fetches and safely evaluates AI-generated JavaScript monkey-patches in the browser before the user experiences logical bugs.

## Usage

Include the script in the `<head>` of your HTML document:

```html
<script src="https://cdn.grumpy.ai/v1/grumpy.js"></script>
<script>
  Grumpy.init({
    apiKey: "YOUR_API_KEY",
    appName: "My Frontend App",
    rescueEngine: true
  });
</script>
```

## Build / Deployment
To deploy this SDK to NPM or a CDN (like unpkg/jsdelivr), simply publish this package:
```bash
npm publish
```
The file `grumpy.js` will automatically become available via jsdelivr and unpkg.
