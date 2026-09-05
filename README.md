# sghoekstra.github.io

Personal academic website of Steven Hoekstra, served by GitHub Pages at <https://sghoekstra.github.io>.

Plain HTML and CSS, no build step. Edit a file, commit, push; GitHub Pages deploys it within a minute or two.

## Layout

| Path | What it is |
| --- | --- |
| `index.html` | Home: bio, job-market notice, research interests, JMP summary, references, contact |
| `research.html` | Job market paper, working papers, work in progress, software, presentations |
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
4. **Work in progress.** Confirm the De Nederlandsche Bank project can be listed publicly.
5. **Job market meetings.** Confirm which meetings you will attend in the notice on `index.html`.
6. **CV.** The PDF in `cv/` is served publicly; remove your home address and phone number from it if you prefer.
7. **Last updated.** The footer date on every page.

## Previewing locally

Open `index.html` in a browser, or run a static server from the repo root:

```sh
python3 -m http.server 8000
```

then visit <http://localhost:8000>.
