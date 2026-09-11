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
| `papers/` | Paper PDFs served by the site |

## To do

1. **Photo.** Replace `assets/img/portrait.svg` with a real photo and update the `<img>` in `index.html` (ideally 4:5 aspect ratio, around 500×625 px).
2. **CV.** The CV still lists the working paper under its old title, *A Dutch Agent Based Model with Optimal Consumption*, and omits the co-authors. The paper is now *Forecasting with a Dutch Agent-Based Model and Optimally Behaving Households*, with Cars Hommes and Frank Pijpers.
3. **Award wording.** Confirm the Society for Computational Economics contest name and outcome on the badge in `research.html`, or remove the badge.
4. **Housing abstract.** That manuscript's abstract is still `TBD`, so the site shows a summary from its introduction, labelled Summary rather than Abstract. Swap in the real abstract when it exists.
5. **Presentations.** Verify the two entries, and decide whether to add the WEHIA 2026 and Ortec talks.
6. **Wage-price abstract.** The posted text is the manuscript abstract with its numeric macros resolved. One trailing `\tbd{...}` marker was dropped; re-check the wording after the final refit.
7. **BeforeIT preprint.** Only the abstract is posted. Add the PDF to `papers/` and link it once the footer names the target journal.
8. **Last updated.** The footer date on every page.

## Previewing locally

Open `index.html` in a browser, or run a static server from the repo root:

```sh
python3 -m http.server 8000
```

then visit <http://localhost:8000>.
