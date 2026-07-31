# AGENTS.md

## Cursor Cloud specific instructions

This repository is a **static frontend** education landing page (HTML, CSS, inline JavaScript). There is no `package.json`, build step, test suite, or linter configuration.

### Running the app locally

Start a static file server from the repository root:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000/` in a browser.

Alternatives: `npx serve /workspace` (often port 3000) or `php -S localhost:8080 -t /workspace`.

### External dependencies

The page loads Tailwind CSS, Google Fonts, DotLottie, and some remote images from CDNs. Network access is required for full styling and animations.

### Lint / test

No lint or test commands are defined in this repo. Verification is manual: confirm the page loads, the **Course** dropdown switches categories and updates the video panel, and FAQ accordions expand.

### Notes

- README mentions Bootstrap 5, but `index.html` uses Tailwind via CDN.
- Font Awesome icon classes (`fa-solid`) are used without a Font Awesome CDN link; some icons may not render locally.
