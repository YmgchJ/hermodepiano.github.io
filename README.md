# Harmodus Piano Website

This repository contains the source code for the official website of **Harmodus Piano**, developed by Sonotech. The website is hosted using GitHub Pages and is accessible at:
[https://harmoduspiano.sonotech.net/](https://harmoduspiano.sonotech.net/)

## Project Structure

The website is built with vanilla HTML, CSS, and JavaScript. It utilizes a simple folder structure for clean URLs without extensions.

```
.
├── index.html           # Landing Page (Top Page)
├── privacy/
│   └── index.html       # Privacy Policy Page
├── contact/
│   └── index.html       # Inquiry / Contact Form Page
├── manual/
│   └── index.html       # User Manual (Placeholder)
├── CNAME                # Custom Domain Configuration
└── README.md            # Project Documentation
```

## Features

- **Modern Aesthetics:** Utilizes a "glassmorphism" design system with elegant typography (Inter, Outfit).
- **Auto-Language Detection:** Pages automatically detect the user's browser language (`navigator.language`). If the browser is set to Japanese, the content automatically switches to Japanese; otherwise, it defaults to English.
- **Contact Form Integration:** The contact form is integrated with [Formspree](https://formspree.io/) for backend-less email forwarding.

## How to Edit

### Modifying the Top Page Text
To edit the main catchphrase or description on the landing page:
1. Open `index.html`.
2. Locate the `<p class="subtitle">` tag inside the `<div class="hero">`.
3. Update the text, save the file, commit, and push.

### Updating the User Manual
1. Open `manual/index.html`.
2. Locate the `<div class="placeholder-box">`.
3. Replace the placeholder with your actual instructions (HTML format).

### Contact Form Setup
To receive emails from the contact form:
1. Create a free account at [Formspree.io](https://formspree.io/).
2. Create a new form and get your unique Endpoint ID (e.g., `mrbgepwk`).
3. Open `contact/index.html`.
4. Locate the form action attribute: `<form action="https://formspree.io/f/YOUR_FORMSPREE_ID" method="POST">`.
5. Replace `YOUR_FORMSPREE_ID` with your actual ID.

## Deployment

Any changes pushed to the `main` branch will be automatically deployed to GitHub Pages. It usually takes a few minutes for the changes to reflect on the live site.

```bash
# To deploy changes:
git add .
git commit -m "your commit message"
git push origin main
```