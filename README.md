# Jinseok Lee — research website

A lightweight, four-page academic website for GitHub Pages. No JavaScript or runtime dependencies are required for the public site.

## Publish

1. Put the contents of this folder in a GitHub repository (the account's `<username>.github.io` repository is suitable).
2. In repository Settings → Pages, choose **GitHub Actions** as the source.
3. Push to the `main` branch, or run the included **Publish research website** workflow.

The workflow rebuilds and publishes the `dist` folder. Relative links support both user and project sites. The site is not yet deployed merely by generating these files.

## Update content

- `content.json`: profile links, current research summaries, publication entries. Optional publication fields: `url`, `pdf`, `code`, `badge`.
- `build.py`: page structure, biography, earlier project descriptions, and news.
- `dist/style.css`: shared design and responsive layout.
- `dist/assets/`: images extracted from the supplied website screenshots.

Run `python build.py` after editing. Open `dist/index.html` to browse locally. No installation is needed.

## Content to confirm before final launch

- Replace screenshot crops with original portrait and research images for higher resolution.
- Add the current CV PDF once supplied; no broken or invented CV download has been added.
- Confirm B.S./M.S. dates if these should be shown.
- Two nanobubble article citations were transcribed from the supplied old website and have no unverified article links.
- Confirm current publication status; 2026 arXiv items are listed as preprints, not as accepted journal articles.
- Older patent claims and unpublished quantitative flow results were not carried over.

## Sources

- User-supplied screenshots of the existing website, September 18, 2026.
- https://arxiv.org/abs/2605.04216
- https://arxiv.org/abs/2605.29424
- https://pubs.aip.org/aip/pof/article/37/2/022146/3336735/Tailored-slip-length-Investigating-the-effect-of
- https://doi.org/10.1017/jfm.2020.791
- https://pubs.acs.org/doi/abs/10.1021/acs.langmuir.2c03027

Typography uses Georgia and system sans-serif fonts, without external font requests. Yale Blue (#00356b) follows https://yaleidentity.yale.edu/guidelines/websites. The proprietary Yale and Mallory fonts are not bundled. Contact is an email link, with no data collection form.

## Research videos

- Confined diffusion: supplied `BF+FL large_1310.05.avi`; converted to H.264 MP4, original 512×512 resolution, 10 fps and 50-second duration retained. No extra speed adjustment. Acquisition frame rate was not supplied, so no physical-time playback factor is claimed.
- Flow deformation: supplied `10%+40%_0.5_30x.mp4`; recompressed as H.264 MP4 at original 640×480 resolution and 29 fps. Existing playback speed retained; 30× caption follows supplied filename. Flow-rate units and mixture ratio are not inferred.
- Both videos have native controls, inline mobile playback, muted audio, poster frames from 5 seconds, and `preload="none"`. No autoplay. Source uploads are unchanged.
- Standalone preview embeds media for portability; deployed pages load separate MP4 files on demand.
