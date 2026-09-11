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
| `cv/` | `cv.tex` and the `Steven_Hoekstra_CV.pdf` it builds, linked from the navigation |
| `papers/` | Paper PDFs served by the site |

## To do

1. **Photo.** Replace `assets/img/portrait.svg` with a real photo and update the `<img>` in `index.html` (ideally 4:5 aspect ratio, around 500×625 px).
2. **Award wording.** Confirm the Society for Computational Economics contest name and whether the result was finalist or winner. The year is now CEF 2026.
3. **Housing abstract.** That manuscript's abstract is still `TBD`, so the site shows a summary from its introduction, labelled Summary rather than Abstract. Swap in the real abstract when it exists.
4. **Presentations.** The Ortec talk and the wage-price short deck have placeholder dates in their sources and are not listed; add them with real venues and years.
5. **Wage-price abstract.** The posted text is the manuscript abstract with its numeric macros resolved. One trailing `\tbd{...}` marker was dropped; re-check the wording after the final refit.
6. **BeforeIT preprint.** Only the abstract is posted. Add the PDF to `papers/` and link it once the footer names the target journal.
7. **Last updated.** The footer date on every page.
## Rebuilding the CV

The CV is written in LaTeX. After editing `cv/cv.tex`, rebuild the PDF the site serves:

```sh
cd cv
pdflatex -jobname=Steven_Hoekstra_CV cv.tex
pdflatex -jobname=Steven_Hoekstra_CV cv.tex   # twice, so page references settle
```

Commit both `cv.tex` and `Steven_Hoekstra_CV.pdf`. Build artefacts are gitignored.

## Previewing locally

Open `index.html` in a browser, or run a static server from the repo root:

```sh
python3 -m http.server 8000
```

then visit <http://localhost:8000>.
