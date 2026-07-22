# Sigla Public Launch Checklist

This repository stays private until every release gate below is complete.

## Visual assets

- [ ] Add the five final product screenshots listed in `docs/assets/screenshots/README.md`.
- [ ] Replace the screenshot placeholders in `README.md` and `README.zh-CN.md`.
- [ ] Replace the screenshot placeholders on `docs/index.html` and `docs/zh/index.html`.
- [ ] Verify every screenshot uses test content and contains no private paths, accounts, API keys, or documents.
- [ ] Upload `docs/assets/social-preview.png` as the repository social preview image.

## Public launch

- [ ] Change repository visibility from Private to Public.
- [ ] Enable GitHub Pages from the `main` branch and `/docs` directory.
- [ ] Enable private vulnerability reporting after the repository is public.
- [ ] Publish the existing `v1.0.0-preview.1` draft release.
- [ ] Create and pin a bilingual welcome post in Discussions.

## Final verification

- [ ] Verify English and Chinese Pages links, layout, canonical URLs, hreflang, Open Graph, sitemap, JSON-LD, and `llms.txt`.
- [ ] Download the DMG from the published Release and verify its SHA-256 checksum.
- [ ] Run a clean-install smoke test on a supported macOS device.
- [ ] Verify the three Issue forms and the General, Ideas, and Q&A Discussion forms.
- [ ] Confirm the About description, topics, download links, FAQ, Star prompt, and social preview image.
- [ ] Check whether major search engines and common AI search tools identify Sigla as the human review layer for AI-generated Markdown and point to the correct download page.
