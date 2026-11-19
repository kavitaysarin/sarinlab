# Sarin Lab Website

Source for **[sarinlab.com](https://sarinlab.com)** — the Sarin Lab, Department of Dermatology, Stanford University School of Medicine. Theme: *Skin as a Sensor for Disease.*

## How it works
- Next.js (App Router) + TypeScript + Tailwind, exported as a static site.
- Every push to `main` builds and deploys to GitHub Pages (`.github/workflows/deploy.yml`), served at the custom domain sarinlab.com.

## Common updates
| To change… | Edit |
|---|---|
| Team members | `src/content/people.ts` (+ headshot in `public/images/team/`) |
| Collaborators | `src/content/collaborators.ts` (+ photo in `public/images/collaborators/`) |
| Selected publications | `src/content/publications.ts` — see `PUBLICATIONS_MAINTENANCE.md` |
| Lab photos | `src/content/gallery.ts` (+ image in `public/images/lab-photos/`) |
| Contact details, homepage stats, social links | `src/content/site.ts` |
| Research / Technologies copy | `src/content/research.ts`, `src/content/technologies.ts` |

Everything in `public/` is publicly downloadable — add only images the site displays, and keep originals offline.

## Local development
```bash
npm ci
npm run dev     # http://localhost:3000
npm run build   # static export → out/
```

## Reference
- Design system (frozen components and tokens): `docs/DESIGN_SYSTEM_FROZEN.md`
- Content rules and project conventions: `CLAUDE.md`
- Deployment: `DEPLOYMENT.md` · Contact form: `CONTACT_FORM_MAINTENANCE.md`
- Open content items: `CONTENT_REVIEW_NEEDED.md`
