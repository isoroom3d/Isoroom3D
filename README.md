# Isoroom3D

A free website teaching how to create isometric rooms using Blender,
MagicaVoxel and other tools — with step-by-step tutorials, a gallery of
examples, and a list of resources.

## Project structure

```
Isoroom3D/
├── index.html              # Home page
├── gallery.html             # Gallery of example scenes
├── resources.html           # Tools, assets and links
├── blog.html                 # Project updates
├── tutorials/
│   ├── index.html                       # Tutorials overview
│   ├── blender-getting-started.html     # Blender part 1
│   └── magicavoxel-getting-started.html # MagicaVoxel part 1
├── css/
│   └── style.css            # Shared styles
├── js/
│   └── main.js               # Mobile nav toggle
└── images/                    # Screenshots, renders, etc.
```

## Running locally

This is a plain static site — no build step needed. Just open `index.html`
in a browser, or run a simple local server for the best experience
(some browsers restrict local file access):

```bash
# from the Isoroom3D folder
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## Adding a new tutorial

1. Copy an existing tutorial file (e.g. `tutorials/blender-getting-started.html`)
   as a starting point — it already has the header, footer and article styles.
2. Update the `<title>`, `<meta description>`, and content inside `.article__body`.
3. Add a card linking to the new page in `tutorials/index.html`.

## Deploying for free (GitHub Pages)

1. Create a free GitHub account if you don't have one.
2. Create a new repository named `Isoroom3D` (or anything you like).
3. Push this folder's contents to the repository.
4. In the repository settings, go to **Pages** and set the source to the
   `main` branch, root folder.
5. Your site will be published at `https://<your-username>.github.io/<repo-name>/`.
