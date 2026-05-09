# SiliconWit.github.io

Source for the SiliconWit GitHub Pages landing at https://siliconwit.github.io.

The page links out to the two main SiliconWit surfaces and to project docs hosted under this org:

- https://siliconwit.com (learning hub: courses, research, blog)
- https://siliconwit.io (IoT/AIoT operations platform)
- https://siliconwit.github.io/deeps/ (DEEPS docs)
- https://siliconwit.github.io/siwit-seal-releases/ (SiliconWit Seal releases)

## Repo layout

```
index.html                          # the entire site (HTML, CSS, JS in one file)
siliconwit-logo-and-trademark.png   # hero logo
ads.txt                             # ad network verification
```

## Preview locally

```
python3 -m http.server 8000
```

Then open http://127.0.0.1:8000/.

## Editing

Everything lives in `index.html`:

- **Hero CTAs**: search for `hero-ctas` and edit the anchor list.
- **About copy**: search for `id="about"`.
- **Core areas**: search for `id="core-areas"`.
- **Timeline**: edit the `timelineData` array near the bottom of the file. Each entry has `year`, `title`, `institution`, `description`, `achievementTitle`, and an `achievements` list. Most recent entries first.
- **Footer links**: search for `<footer`.

## Deploy

Pushing to `main` publishes to GitHub Pages automatically.
