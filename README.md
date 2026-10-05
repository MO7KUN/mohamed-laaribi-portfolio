# Mohamed Laaribi — Portfolio

A responsive personal portfolio for **Mohamed Laaribi**, presenting his work in AI and machine learning, NLP, data engineering, and full-stack development. Built with semantic HTML, Tailwind CSS, and a small amount of vanilla JavaScript.

## Run locally

1. Install [Node.js](https://nodejs.org/) (LTS).
2. From this folder, install the development dependency:

   ```sh
   npm install
   ```

3. Build the Tailwind stylesheet:

   ```sh
   npm run build
   ```

4. Open `index.html` in a browser, or serve this folder with any static file server. During development, run `npm run watch:css` to rebuild CSS as you edit.

The checked-in `src/output.css` is a ready-to-view stylesheet. Rebuilding it uses the Tailwind configuration and `src/input.css`.

## Publish with GitHub Pages

1. Create a GitHub repository and upload the contents of this folder.
2. In the repository, open **Settings → Pages** and set **Source** to **GitHub Actions**.
3. The included workflow installs dependencies, builds Tailwind CSS, and publishes the site whenever you push to the `main` branch. You can also run it from the Actions tab.

The site is static and needs no server. The contact form opens a prefilled email draft addressed to `mohamedlaaribi45@gmail.com`; it does not transmit or store submissions. A visitor needs an email app configured to send the message. To accept messages without that, configure a form service and update the form handling in `src/main.js`.

## Automatic GitHub projects

The projects section loads all public repositories belonging to `MO7KUN` from GitHub's public API on each page load, with newest repositories first. Pagination supports accounts with more than 100 repositories. Public forks and archived projects are included; private and disabled repositories are excluded. Create a public repository, add a description, and it will appear when visitors open or refresh the portfolio without editing or rebuilding the site. GitHub Projects boards are not repositories and are not imported. The featured CV projects remain visible if GitHub is unavailable or its API rate limit is reached; visitors can use the link to the GitHub profile.

No access token or backend is needed. Repository descriptions and programming languages come directly from GitHub.

## Personalize

- Edit the page content in `index.html`.
- Edit responsive styling and Tailwind directives in `src/input.css`.
- Adjust Tailwind theme and content scanning in `tailwind.config.js`.
- Update mobile navigation and contact form behavior in `src/main.js`.
- Replace or add project links when public repositories or demos are available.

## Accessibility and performance

Includes a skip link, semantic landmarks, labelled form fields, keyboard-operable navigation, visible focus states, reduced-motion support, responsive layout, and descriptive metadata. Google Fonts are loaded remotely; the page falls back to system sans-serif fonts when unavailable.

## Project structure

```text
.
├── .github/workflows/pages.yml
├── assets/favicon.svg
├── index.html
├── package.json
├── tailwind.config.js
└── src/
    ├── input.css
    ├── main.js
    └── output.css
```
