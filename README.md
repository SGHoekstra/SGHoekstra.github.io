# sghoekstra.github.io

Personal academic website of Steven Hoekstra, served by GitHub Pages at <https://sghoekstra.github.io>.

Plain HTML and CSS, no build step. Edit a file, commit, push; GitHub Pages deploys it within a minute or two.

## Layout

| Path | What it is |
| --- | --- |
| `index.html` | Home: bio, research interests, research list, education, experience, references, contact |
| `research.html` | Working papers, work in progress, research programme, software, presentations, theses |
| `teaching.html` | MSc lecture series, Tinbergen guest lecturing, thesis supervision and undergraduate tutorials |
| `assets/css/style.css` | The only stylesheet |
| `assets/img/` | Portrait and favicon |
| `cv/` | `cv.tex` and the `Steven_Hoekstra_CV.pdf` it builds, linked from the navigation |
| `papers/` | Paper PDFs served by the site |

## To do

1. **Photo.** Replace `assets/img/portrait.svg` with a real photo and update the `<img>` in `index.html` (ideally 4:5 aspect ratio, around 500×625 px).
2. **Work-in-progress summaries.** Housing and wage–price summaries reflect the redesigned projects as of October 2026. Update them when integration, calibration and the new experiments yield reportable results.
3. **Lecture slides.** In the course repo, `lecture_1_intro_abm` and `lecture_2_sfc_abm` were committed as nested-repository pointers, so they are empty on GitHub and the slides are not online. Push the PDFs, then link them under Lectures on the teaching page.
4. **Presentations.** The Ortec talk and the wage-price short deck have placeholder dates in their sources and are not listed; add them with real venues and years.
5. **BeforeIT preprint.** Only the abstract is posted. Add the PDF to `papers/` and link it once the footer names the target journal.
6. **Last updated.** Update the footer date on every page when changing public content.

Award wording was verified against the [CEF 2026 Graduate Student Paper Award announcement](https://comp-econ.com/cef-2026-student-paper/): Steven Hoekstra was a runner-up.

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
