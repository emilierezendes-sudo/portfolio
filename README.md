# Editing this site

This is a plain [Jekyll](https://jekyllrb.com) site. GitHub builds and publishes it
automatically every time you save a change here — no software to install, no Claude
Code required. Everything below can be done in GitHub's own web editor: open a file,
click the pencil icon, edit, commit.

## Where things live

| Want to change...                              | Edit this file            |
|-------------------------------------------------|----------------------------|
| Home page bio / tagline / headshot               | `index.md` (top of file)  |
| Experience timeline (add/edit a job)             | `_data/experience.yml`    |
| Project case studies                             | `_data/projects.yml`      |
| "More work" cards on the Projects page           | `_data/more_work.yml`     |
| Skills grid on Home                              | `_data/skills.yml`        |
| Testimonials                                     | `_data/testimonials.yml`  |
| Resume page text / highlights                    | `resume.md` (top of file) |
| Resume PDF file itself                           | replace `Emilie-Rezendes-Resume.pdf`, keep the same filename |
| Photos / PDFs                                    | `assets/` folder          |

The `_data/*.yml` files are simple lists — copy the shape of an existing entry, change
the words, keep the same indentation. For example, to add a new job to
`_data/experience.yml`, copy one whole entry (from its `- role:` line to just before the
next `- role:` line) and edit the copy.

## Adding or swapping a photo

1. Upload the new image file into `assets/` (via GitHub's "Add file" button).
2. In the relevant `_data/*.yml` file (or `index.md` for the headshot), change the
   `image:` (or `portrait:`) value to `assets/your-new-filename.png`.

## Things you shouldn't need to touch

`_layouts/`, `_includes/`, and `assets/style.css` hold the page structure and visual
design (colors, fonts, spacing) shared across every page. You can leave these alone —
editing the files above is enough for basically everything short of a redesign.

## If something looks broken after a save

GitHub takes 30–60 seconds to rebuild after you commit. If the site still looks wrong
after that, check the **Actions** tab on this repo — a red ✗ next to "pages build and
deployment" means something in a `.yml` or `.md` file has a formatting mistake (usually
a missing quote or wrong indentation). The error message there names the file and line.
