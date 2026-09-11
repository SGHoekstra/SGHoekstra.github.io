# sghoekstra.github.io

Personal academic website of Steven Hoekstra, served by GitHub Pages at <https://sghoekstra.github.io>.

Plain HTML and CSS, no build step. Edit a file, commit, push; GitHub Pages deploys it within a minute or two.

## Layout

| Path | What it is |
| --- | --- |
| `index.html` | Home: bio, research interests, research list, education, experience, references, contact |
| `research.html` | Working papers, work in progress, software, presentations, theses |
| `teaching.html` | Teaching experience |
| `assets/css/style.css` | The only stylesheet |
| `assets/img/` | Portrait and favicon |
| `cv/` | `Steven_Hoekstra_CV.pdf`, linked from the navigation |
| `papers/` | Paper PDFs, once there are any to post |

## To do

1. **Photo.** Replace `assets/img/portrait.svg` with a real photo and update the `<img>` in `index.html` (ideally 4:5 aspect ratio, around 500×625 px).
2. **Paper 1 PDF.** When *A Dutch Agent-Based Model with Optimal Consumption* is final, put the PDF in `papers/` and link it from its entry in `research.html`.
3. **Award wording.** Confirm the Society for Computational Economics contest name and outcome on the badge in `research.html`, or remove the badge.
4. **Housing abstract.** That manuscript's abstract is still `TBD`; the site currently shows a summary written from its introduction. Swap in the real abstract when it exists.
5. **Presentations.** Verify the two entries, and decide whether to add the WEHIA 2026 and Ortec talks.
6. **Last updated.** The footer date on every page.

## Previewing locally

Open `index.html` in a browser, or run a static server from the repo root:

```sh
python3 -m http.server 8000
```

then visit <http://localhost:8000>.
