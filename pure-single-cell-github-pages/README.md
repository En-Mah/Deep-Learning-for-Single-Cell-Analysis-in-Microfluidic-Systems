# Deep Learning for Single-Cell Analysis — PURE 2026

A responsive, static research project website for **Mahla Entezari's 2026 Sabancı University PURE internship**.

**Project:** Deep Learning for Single-Cell Analysis in Microfluidic Systems  
**Research supervisors:** Prof. Dr. Erchan Aptoula and Assoc. Prof. Dr. Meltem Elitas Hartmann  
**Internship:** July 6 – August 20, 2026

## Files

```text
pure-single-cell-site/
├── index.html                  # All website content
├── styles.css                  # Responsive design, typography, UI styles
├── .nojekyll                   # Prevents GitHub Pages from running Jekyll
├── README.md                   # You are here
└── assets/
    ├── favicon.svg
    ├── microscopy-raw.webp     # Crop of the author's project-report Figure 7
    ├── microscopy-tracked.webp # Crop of the author's project-report Figure 7
    ├── microscopy-masks.webp   # Additional figure crop
    ├── tracking-comparison.webp
    ├── research-report.pdf
    └── project-poster.pdf
```

Everything is static HTML and CSS. There are no JavaScript dependencies, frameworks, build tools, or server-side requirements. The site loads Google Fonts with local fallback fonts.

## Publish on GitHub Pages

1. On GitHub, create a **public** repository. For a portfolio page at `https://YOUR_USERNAME.github.io/`, name the repository `YOUR_USERNAME.github.io`. For a project page, use any repository name such as `pure-single-cell`; the URL will be `https://YOUR_USERNAME.github.io/pure-single-cell/`.
2. Upload the **contents** of this folder to the root of that repository (including the `assets` folder, `index.html`, `styles.css`, and `.nojekyll`). Or clone the repository locally, copy the contents in, commit, and push to `main`.
3. Go to the GitHub repository's **Settings → Pages**. Under **Build and deployment**, select **Deploy from a branch**, then select the `main` branch and `/ (root)` folder; save.
4. Open the published Pages URL once GitHub finishes deployment.

No configuration changes are needed for either a user site or a project subpath: all local links use relative paths.

## Edit your details

- Update text and numerical results in `index.html`.
- Change palette, spacing and layout in `styles.css` (`:root` contains the main colors).
- The contact link at the bottom is the public address printed in the project report: `MahlaEntezariii@gmail.com`. Change or remove it if you don't want it publicly displayed.
- To add a profile or social link, insert it in `<div class="footer-links">` near the end of `index.html`.
- Replace the local PDFs under `assets/` if you want to publish updated or redacted versions.

**Public disclosure note:** The report and collaborative poster are included as convenient local downloads. Before publishing, confirm that your supervisors and collaborators approve sharing any unpublished scientific work, figures, or data. The completion certificate is intentionally **not** bundled, because it contains identifiable administrative verification information.

## Scientific accuracy notes

- The 29-frame **Trackastra** benchmark and 141-frame **OmniSegger/Omnipose** reproduction are separate experiments.
- The Trackastra TRA comparison uses the **same** tracking approach with ground-truth versus predicted segmentation masks.
- The Bactrack tracking and division F1 values reflect **agreement between outputs from two input-mask sets**, and should not be represented as an independently annotated accuracy benchmark.
- The website presents Mahla's documented benchmarking/reproduction work separately from the wider collaboration's CiproSeg work.
- Figures are derived from the project report and should retain the project attribution when reused.

## Tested layout

Responsive breakpoints are included for desktop, tablet, and mobile, along with accessibility and reduced-motion support.
