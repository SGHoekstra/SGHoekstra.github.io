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
| `cv/` | Put `Steven_Hoekstra_CV.pdf` here (the nav links to it) |
| `papers/` | Put `Hoekstra_JMP.pdf` and `Hoekstra_JMP_slides.pdf` here |

## Before going live

Search the HTML for `TODO` and for text in `[square brackets]`. Each one marks something to fill in or confirm:

1. **Photo.** Replace `assets/img/portrait.svg` with a real photo and update the `<img>` in `index.html` (ideally 4:5 aspect ratio, around 500×625 px).
2. **CV and paper PDFs.** Add the files listed above, or change the links.
3. **References.** Fill in advisors and letter writers on `index.html`.
4. **Job market paper.** Replace the draft abstract in `research.html` with the one from the paper, confirm the co-author line, and check the wording of the SCE contest award.
5. **Working papers, work in progress, presentations, teaching.** Replace the bracketed template entries or delete the sections you do not need.
6. **Job market meetings.** Confirm which meetings you will attend in the notice on `index.html`.
7. **Last updated.** The footer date on every page.

## Previewing locally

Open `index.html` in a browser, or run a static server from the repo root:

```sh
python3 -m http.server 8000
```

then visit <http://localhost:8000>.
