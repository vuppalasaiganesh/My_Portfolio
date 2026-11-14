# My Portfolio

Personal portfolio of **Sai Ganesh Vuppala**: AI Architect, AWS Solutions Architect, Amazon Connect Architect and Developer, DevOps Engineer.

A static, five-page site (Index, Work, Career, Capabilities, Résumé, Contact) with scroll-driven transitions built on GSAP, ScrollTrigger and Lenis. There is no build step.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The whole site: markup, styles and scripts. Comments mark each ScrollTrigger setup. |
| `sai.jpg` | Portrait on the Index page. Replace with any 4:5 photo. |
| `surya-simha.jpg` | Render shown for the Surya Simha project. |
| `SaiGanesh_Vuppala_Resume.pdf` / `.docx` | Résumé, linked from the Résumé page. |

## Run locally

```bash
python3 -m http.server 8000
```

Open http://localhost:8000. Libraries load from cdnjs and jsDelivr, so an internet connection is needed for the animation; without it the pages still read normally.

## Live site

https://vuppalasaiganesh.github.io/My_Portfolio/

## Deploy

`.github/workflows/pages.yml` publishes the repository to GitHub Pages on every push to `main`. One-time setup: Settings, Pages, Source, **GitHub Actions**.

## Visitor analytics

Visits are counted with [GoatCounter](https://www.goatcounter.com) under the site code `vuppalasaiganesh` (set as `GC_CODE` in `index.html`). It loads only on the github.io site, sets no cookies and stores no personal data.

What the dashboard shows:

- **Page views** per page: `/home`, `/work`, `/career`, `/stack`, `/resume`, `/contact`
- **Where visitors came from**: referrer sites, plus `resume-qr` (scanned the résumé QR code) and `resume-link` (clicked the link in the PDF)
- **Browser, OS, screen size, country** and, if enabled in GoatCounter settings, region and language
- **Events**: `work/<project>` (scrolled to a project), `resume/download`, `resume/read-to-end`, `contact/saw-details`, `contact/copy-email`, `contact/copied-email`, `contact/copied-phone`, `contact/phone`, `click/linkedin`, `click/github...`, `click/traddx`, `time/30s`, `time/2m`, `time/5m`, `time/10m`

Tag any link you share with `?ref=`, for example `https://vuppalasaiganesh.github.io/My_Portfolio/?ref=linkedin`, and it shows up as its own source.

## Replacing placeholders

- Project mockups labelled "Illustration" can be swapped for real screenshots: replace the `.mock` block in that project with `<div class="shot"><img src="your-shot.jpg" alt="..."></div>`.
- After changing the résumé text, update the Résumé page text and the PDF together.
