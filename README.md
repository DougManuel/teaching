# Teaching

Lecture materials by Doug Manuel, written in [Quarto](https://quarto.org) so that slides, data and calculations live in one reproducible source.

## Lectures

| Folder | Course | Topic |
|---|---|---|
| `calibration/` | EPI 6101 An Introduction to Machine Learning (University of Ottawa) | Calibration and discrimination: a worked example at the bus stop |

## Rendering

Each lecture renders on its own. From the repository root:

```bash
quarto render calibration/bus-stop-worked-example.qmd
```

The output is a single reveal.js HTML file. Rendering needs R with the `knitr`, `ggplot2` and `survival` packages (`survival` ships with R). Equations load MathJax from the web, so the slides need an internet connection to display them.

Rendered slides and PDFs for each lecture, as presented, are attached to the [releases](https://github.com/DougManuel/teaching/releases). Release tags name the lecture and year, for example `calibration-2026`.

## Shared theme

`theme/teaching.scss` holds the common slide styling. Lectures reference it so that colours and fonts change in one place.

## Licence

Text, slides, figures and data: [CC BY 4.0](LICENSE-CC-BY-4.0.txt). Code: [MIT](LICENSE-MIT.txt). See [LICENSE.md](LICENSE.md).
