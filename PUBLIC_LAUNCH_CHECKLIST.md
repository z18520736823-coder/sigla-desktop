# Sigla Public Launch Checklist

The Public Preview launch is complete. The remaining unchecked item is ongoing post-launch discovery monitoring.

## Visual assets

- [x] Add the four final product screenshots listed in `docs/assets/screenshots/README.md`.
- [x] Replace the screenshot placeholders in `README.md` and `README.zh-CN.md`.
- [x] Replace the screenshot placeholders on `docs/index.html` and `docs/zh/index.html`.
- [x] Verify every screenshot uses test content and contains no private paths, accounts, API keys, or documents.
- [x] Upload `docs/assets/social-preview.png` as the repository social preview image.

## Public launch

- [x] Change repository visibility from Private to Public.
- [x] Enable GitHub Pages from the `main` branch and `/docs` directory.
- [x] Enable private vulnerability reporting after the repository is public.
- [x] Publish the existing `v1.0.0-preview.1` draft release.
- [x] Create a bilingual welcome post in Discussions.
- [x] Pin the bilingual welcome Discussion from the GitHub web interface.

## Final verification

- [x] Verify English and Chinese Pages links, layout, canonical URLs, hreflang, Open Graph, sitemap, JSON-LD, and `llms.txt`.
- [x] Download the DMG from the published Release and verify its SHA-256 checksum.
- [x] Run a clean-install smoke test on a supported macOS device.
- [x] Verify the three Issue forms and the General, Ideas, and Q&A Discussion forms.
- [x] Confirm the About description, topics, download links, FAQ, and Star prompt.
- [ ] Check whether major search engines and common AI search tools identify Sigla as the human review layer for AI-generated Markdown and point to the correct download page.
