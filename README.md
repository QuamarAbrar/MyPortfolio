<div align="center">

# Quamar Abrar — Portfolio

An expressive portfolio for identities, interfaces, and visual stories.
Built with React, TypeScript, and GSAP.

[Explore the source](src/) · [Browse project data](src/data.ts) · [Getting started](#getting-started)

</div>

<br />

<table>
  <tr>
    <td width="34%"><img src="src/assets/optimized/posters/01-veil.webp" alt="VEIL editorial poster study" /></td>
    <td width="33%"><img src="src/assets/optimized/posters/02-recode.webp" alt="RE:CODE poster study" /></td>
    <td width="33%"><img src="src/assets/optimized/posters/04-redbull.webp" alt="Red Bull — Flat Out poster study" /></td>
  </tr>
</table>

<p align="center"><sub>Selected poster studies from the portfolio · <a href="src/assets/optimized/posters/">View all artwork</a></sub></p>

## The experience

A motion-led portfolio designed around a warm paper-and-green palette, expressive type, and clear editorial rhythm. The page brings together selected digital projects, mobile product concepts, poster work, and packaging.

- **Seven featured digital projects** with links to their live experiences.
- **Interactive mobile showcases** for KOMA and VEIL, with navigable product screens.
- **Poster and packaging galleries** featuring original portfolio artwork.
- **Responsive motion design** with GSAP and ScrollTrigger, tailored to pointer, touch, and reduced-motion preferences.
- **Canvas preloader** with a skip control and a reduced-motion alternative.

## Built with

| Layer | Tools |
| --- | --- |
| UI | React 19, TypeScript |
| Build | Vite 8 |
| Motion | GSAP 3, ScrollTrigger |
| Styling | CSS, Tailwind CSS 4 |
| Typography | Alata, Cardo |

## Getting started

This project uses Node.js 22 and pnpm. Large image assets are tracked with Git LFS.

```bash
git lfs install
git clone https://github.com/QuamarAbrar/MyPortfolio.git
cd MyPortfolio
git lfs pull
pnpm install
pnpm dev
```

Vite serves the development site at `http://localhost:8443`.

```bash
pnpm build       # Create the production bundle in dist/
pnpm preview     # Preview the production bundle locally
pnpm format      # Format source files with oxfmt
```

## Make it yours

- **Projects and gallery content:** edit `src/data.ts` to change project titles, descriptions, links, and artwork.
- **Visual identity:** adjust the CSS custom properties near the top of `src/index.css` for colors, type, spacing, and shape.
- **Site metadata:** update `.figma/make/site.json` for the document title, description, language, and optional social metadata.
- **Images:** replace files in `src/assets/optimized/` and keep descriptive alt text in the corresponding data or components. The original source artwork is also retained in `src/assets/`.

The featured project URLs, portrait, and portfolio artwork are specific to Quamar Abrar. Replace those with your own approved content before reusing this as a starter. Keep image rights and attribution in mind when publishing.

## Motion and accessibility

The interface keeps native scrolling in control while GSAP animates selected transitions and scroll-linked details. Touch layouts reduce desktop choreography, and reduced-motion preferences bypass the particle preloader and motion-heavy effects. Interactive controls include labels and explicit navigation for the mobile showcases.

## Project layout

```text
src/
├── assets/
│   ├── optimized/     # WebP artwork used by the site
│   └── ...            # Source images
├── App.tsx            # Page sections and interactions
├── data.ts            # Projects and gallery content
└── index.css          # Design tokens, layout, and responsive styles
.figma/make/site.json  # Site metadata used by the Vite config
```
