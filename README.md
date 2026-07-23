# Rae-Anne Richardson — Portfolio

Single-page interactive portfolio. Eight campaigns plotted on a world map, with full case studies below.

## Files to upload

| File | Purpose |
|---|---|
| `index.html` | The entire site — HTML, CSS and JS in one file |
| `cubby.jpg` | CUBBY Cargo |
| `otc.jpg` | Trinidad & Tobago National Pavilion |
| `noble.jpg` | Noble Marine Cadet Scholarship |
| `mawi.jpg` | MAWI |
| `forbes.jpg` | Freight Without Friction |
| `usine.jpg` | L'Usine Nouvelle |
| `republic.jpg` | Take Your Shot to Win |
| `global.jpg` | Global brand campaigns |
| `CV.pdf` | **You need to add this** — the Download CV button links to it |

All files must sit in the same folder, at the repository root.

## Publishing on GitHub Pages

1. Create a new repository (a name like `portfolio` is fine).
2. Upload every file above to the repository root.
3. Go to **Settings → Pages**.
4. Under *Source*, choose **Deploy from a branch**, select `main` and `/ (root)`, then **Save**.
5. Wait a minute or two. The site appears at `https://<your-username>.github.io/<repository-name>/`

For a custom domain, add it under Settings → Pages → Custom domain, then point a CNAME
record at `<your-username>.github.io` with your domain registrar.

## Editing content

Everything in the case studies is driven by the `PORTS` array inside the `<script>` block in `index.html`:

- `title`, `kick`, `year` — headings and labels
- `body` — the paragraph
- `points` — the bullet list (`<strong>` and links are allowed)
- `img` / `cap` — image filename and its caption
- `lat` / `lon` — map position; leave alone unless the location changes

Client and press names live in the `#clients` section of the HTML, not in the script.

## Swapping an image

Put the new file in this folder (landscape, roughly 4:3, under ~400KB),
then change `img:"oldfile.jpg"` to `img:"newfile.jpg"` on the matching entry.
