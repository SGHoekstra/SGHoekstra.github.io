# sghoekstra.github.io

Personal academic website of Steven Hoekstra, served by GitHub Pages at <https://sghoekstra.github.io>.

Plain HTML and CSS, no build step. Edit a file, commit, push; GitHub Pages deploys it within a minute or two.

## Layout

| Path | What it is |
| --- | --- |
| `index.html` | Home: bio, research interests, JMP summary, education, experience, references, contact |
| `research.html` | Job market paper, work in progress, software, presentations, theses |
| `teaching.html` | Teaching experience |
| `assets/css/style.css` | The only stylesheet |
| `assets/img/` | Portrait and favicon |
| `cv/` | `Steven_Hoekstra_CV.pdf`, linked from the navigation |
| `papers/` | Put `Hoekstra_JMP.pdf` and `Hoekstra_JMP_slides.pdf` here |

## Before going live

Search the HTML for `TODO`. Each one marks something to fill in or confirm:

1. **Photo.** Replace `assets/img/portrait.svg` with a real photo and update the `<img>` in `index.html` (ideally 4:5 aspect ratio, around 500×625 px).
2. **Paper PDFs.** Add `papers/Hoekstra_JMP.pdf` and `papers/Hoekstra_JMP_slides.pdf`, or change the links.
3. **Job market paper.** Confirm the co-author line and the wording of the SCE contest award in `research.html`.
4. **Work in progress.** Titles and authors now come from the manuscripts. Replace each summary with the paper's own abstract once it is written, and pick one title for the wage-price paper.
5. **Last updated.** The footer date on every page.

## Previewing locally

Open `index.html` in a browser, or run a static server from the repo root:

```sh
python3 -m http.server 8000
```

then visit <http://localhost:8000>.
