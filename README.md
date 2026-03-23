# Jagjot Singh Portfolio (React + Vite)

Personal portfolio website for Jagjot Singh built with React, Vite, Tailwind CSS, and Framer Motion. The site highlights skills, education and credentials, featured projects, and contact information with a modern animated UI.

## Tech Stack
- React 18 with Vite
- Tailwind CSS + tailwindcss-animate
- Framer Motion for animations
- Lucide icons

## Getting Started
1. Install dependencies:
   ```bash
   npm install
   ```
2. Run the dev server:
   ```bash
   npm run dev
   ```
   Open the local URL shown in the terminal.
3. Build for production:
   ```bash
   npm run build
   ```
4. Preview the production build:
   ```bash
   npm run preview
   ```

## Project Structure
- `src/App.jsx` — main page layout and section composition.
- `src/components/Navbar.jsx` — top navigation (Home, Skills, Education, Projects, Contact).
- `src/components/Hero.jsx` — intro, profile image, and primary social/contact CTAs.
- `src/components/Services.jsx` — skills overview (languages, libraries, tools, soft skills).
- `src/components/WorkExperience.jsx` — education, training, certifications, and achievements.
- `src/components/Projects.jsx` — featured project cards and GitHub links.
- `src/components/Contact.jsx` — contact form and direct contact channels.
- `src/components/Footer.jsx` — footer links and profile credits.
- `src/components/CoffeeCounter.jsx` — interactive coffee counter widget.
- `src/components/ui/` — shared UI primitives (button, card, input, textarea, lamp, encrypted-text).
- `src/context/ThemeContext.jsx` — light/dark theme state and toggle hook.
- `src/index.css` — Tailwind base plus custom styles.

## Notable Features
- Dark/light theme toggle powered by context.
- Lazy-loaded heavy sections to improve initial load.
- Animated interactions with Framer Motion (hero text, cards, buttons, contact form feedback).
- Coffee counter with localStorage persistence and playful particles.
- Responsive design with smooth scrolling and animated backgrounds.

## Resume Mapping
- Hero: Name, headline, and quick links (GitHub, LinkedIn, email).
- Skills: Languages, frameworks/libraries, platforms/tools, soft skills.
- Education and Credentials: Education timeline, training, certificates, achievements.
- Projects: Weather dashboard, Hotel dashboard, Library management system, Quiz it Up.
- Contact: Email, phone, location, social profile links.

## Customize Content
- Update personal details in:
   - `src/components/Hero.jsx`
   - `src/components/Contact.jsx`
   - `src/components/Footer.jsx`
- Update skill cards in:
   - `src/components/Services.jsx`
- Update education/certificates section in:
   - `src/components/WorkExperience.jsx`
- Update project cards and repository links in:
   - `src/components/Projects.jsx`
- Update profile image by replacing:
   - `public/me.png`

## Deployment
- Static build output lives in `dist/` after `npm run build`.
- The repo includes a `deploy` script for GitHub Pages (`npm run deploy`) using `gh-pages`; update `base` in `vite.config.js` if deploying to a subpath.

## Scripts
- `npm run dev` — start local dev server.
- `npm run build` — production build.
- `npm run preview` — preview the production build locally.
- `npm run deploy` — publish `dist/` to GitHub Pages (runs build first).

## Notes
- Minification uses Terser; if you prefer esbuild, change `build.minify` in `vite.config.js`.
- Tailwind is configured in `tailwind.config.js`; PostCSS in `postcss.config.js`.
