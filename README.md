# Minimal Portfolio Template

A simple one-page portfolio in light blue, black, white and light green. No frameworks, no build step. It switches to a dark version automatically when the visitor's device is in dark mode.

## What's inside

```
portfolio-site/
├── index.html   # content + tab script
├── style.css    # colors, fonts, layout
└── README.md
```

## Sections

- **Status:** what you are looking for right now
- **My story:** your journey as a timeline
- **Experience:** three tabs (Professional, Volunteer, Personal projects)
- **GitHub:** pinned repositories
- **CV:** download button
- **Contact:** email and social links

## Run it

Open `index.html` in your browser. That's it. Keep `index.html` and `style.css` in the same folder.

Fonts load from Google Fonts, so you need to be online to see them. Without a connection, the page falls back to your system fonts.

## Make it yours

1. **Name and title:** search for `Your Name` in `index.html` and replace it (it appears in the page title, the nav, the heading and the footer).
2. **Status:** edit the block under `<!-- STATUS -->`: the heading, the sentence and the Role, Type, Location and Available lines. Change the "Open to work" label if it no longer applies.
3. **Story:** edit the items under `<!-- STORY -->`. Copy one `<li>...</li>` to add a step.
4. **Experience:** edit the items under `<!-- EXPERIENCE -->`. Each tab has its own panel. Copy one `<div class="item">...</div>` to add an entry.
5. **GitHub:** replace `yourname` and the repo names in the links under `<!-- GITHUB -->`.
6. **CV:** put your PDF in the same folder (for example `cv.pdf`) and change `href="#"` in the CV button to `href="cv.pdf"`.
7. **Contact:** replace `you@example.com` and the LinkedIn, GitHub and Telegram links.

## Add your own pictures

Each story step and experience entry has a small picture tile with an emoji:

```html
<div class="pic">🌱</div>
```

To use a real photo, logo or screenshot, save the image in the same folder (for example `photo.jpg`) and replace the emoji:

```html
<div class="pic"><img src="photo.jpg" alt="Short description"></div>
```

The image is cropped to fill the tile automatically. Square images work best.

## Change the colors

Open `style.css` and edit the variables at the top:

| Variable | Used for |
| --- | --- |
| `--blue` | tab bar, tags, light blue tiles |
| `--blue-strong` | timeline line, repo card borders |
| `--green` | status card, buttons, light green tiles |
| `--green-strong` | status dot, underline, repo language dot |
| `--ink` | headings, outlines, black |
| `--bg` | page background |

The dark mode colors are in the two blocks right below, under `prefers-color-scheme: dark` and `data-theme="dark"`.

## Put it online (free)

- **GitHub Pages:** push the folder to a repo, then go to Settings → Pages and choose the main branch.
- **Netlify:** drag and drop the folder at app.netlify.com/drop.
- **Vercel:** import the repo and deploy. No settings needed.

## License

Free to use and change for your own portfolio.
