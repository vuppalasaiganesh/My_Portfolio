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

## Deploy

`.github/workflows/pages.yml` publishes the repository to GitHub Pages on every push to `main`. One-time setup: Settings, Pages, Source, **GitHub Actions**.

## Replacing placeholders

- Project mockups labelled "Illustration" can be swapped for real screenshots: replace the `.mock` block in that project with `<div class="shot"><img src="your-shot.jpg" alt="..."></div>`.
- After changing the résumé text, update the Résumé page text and the PDF together.
