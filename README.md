# AJIBOYE OLUWASEYI | Software Developer Portfolio

A personal portfolio website presenting my work, experience, skills, and ways to get in touch. Built as a static, responsive site with a lightweight frontend and no application server requirement.

## About this project

This repository contains one of my portfolio website implementations. It combines a professional landing page with project discovery, resume access, and a contact experience. The project is designed to make it easy for visitors and recruiters to understand my work and explore selected repositories.

## Highlights

- Responsive layout for desktop and mobile screens
- Dark mode with system preference support and a manual toggle
- Project section that reads public repository information from the GitHub API
- Resume view and download links
- Contact form configured for Netlify Forms
- Semantic HTML and search-oriented metadata

## Screenshots

There are no dedicated screenshots in the repository at present. Add authentic captures under `docs/screenshots/` and link them here when ready.

## Technology

- HTML
- CSS, including Tailwind utility styles
- JavaScript
- GitHub REST API for public repository data
- Netlify Forms for deployed contact submissions

## Run locally

Install dependencies and start the local development server:

```bash
npm install
npm run dev
```

Open the local address printed by the development server.

## Personalization

Before using this project as a template, review and update:

- Name, introduction, and profile image in `index.html`
- GitHub username and social links
- Resume PDF and its links
- Contact form settings for the intended host
- Repository links and project descriptions

## Deployment

The project includes Netlify configuration. Netlify is the intended host for the contact form integration; that form will not submit through Netlify Forms when hosted elsewhere without replacing it with a compatible service. Review the provider settings and the repository configuration before deploying.

## Notes

The repository currently includes a `node_modules/` directory. For a cleaner, reproducible project, dependencies should generally be installed from the package manifest rather than committed with the application source.

## Author

**Ajiboye Oluwaseyi** · [GitHub](https://github.com/ajiboy-dev)
