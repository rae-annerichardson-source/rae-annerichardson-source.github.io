# Rae-Anne Richardson — Portfolio

Single-page interactive portfolio. Nine campaigns plotted on a world map, with full case studies below.

## Files (all must sit at the repository root)

| File | Purpose |
|---|---|
| `index.html` | The entire site — HTML, CSS and JS in one file |
| `CV.pdf` | Linked from the Download CV button |
| `cubby.jpg` | CUBBY Cargo |
| `otc.jpg` | Trinidad & Tobago National Pavilion |
| `enps.jpg` | Rebuilding belief from the inside |
| `noble.jpg` | Noble Marine Cadet Scholarship |
| `mawi.jpg` | MAWI |
| `forbes.jpg` | Freight Without Friction |
| `usine.jpg` | L'Usine Nouvelle |
| `republic.jpg` | Take Your Shot to Win |
| `global.jpg` | Global brand campaigns |

## Publishing

The repository is named `rae-annerichardson-source.github.io`, so GitHub Pages
serves it at the root: https://rae-annerichardson-source.github.io/

Settings → Pages → Source: Deploy from a branch → `main` → `/ (root)`.

Changes go live a minute or two after pushing. Hard-refresh (Ctrl/Cmd+Shift+R)
to get past browser caching, especially for images and the PDF.

## Editing content

Case studies are driven by the `PORTS` array inside the `<script>` block:

- `title`, `kick`, `year` — headings and labels
- `body` — the paragraph
- `points` — the bullet list (`<strong>` and links allowed)
- `img` / `cap` — image filename and caption
- `lat` / `lon` — map position; leave alone unless the location changes
- `sharesPin` — set when a campaign shares another entry's map marker

Order in the array sets the order on the page and in the port index.

Client and press names live in the `#clients` section of the HTML, not the script.

## Notes

- Mobile breakpoints at 900px, 760px, 640px and 380px. On phones the map is a
  visual anchor and the port index below it is the navigation, because several
  ports sit only a few pixels apart at that width.
- Swapping an image: keep the same filename, or update `img:` on the entry.
