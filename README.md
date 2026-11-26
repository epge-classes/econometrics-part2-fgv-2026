# Econometrics I (Part II): Econometrics and Causal Inference @ FGV EPGE - 2026

Repository for the second half of Econometrics I (*Econometrics and Causal Inference*), taught by [Valdemar Pinho Neto](https://sites.google.com/view/valdemarneto/home). The first half is taught by [Raul Riva](https://epge-classes.github.io/econometrics-fgv-2026/).

<table>
  <tr><td><b>Instructor</b></td><td>Valdemar Rodrigues de Pinho Neto (<a href="mailto:valdemar.pinho@fgv.br">valdemar.pinho@fgv.br</a>)</td></tr>
  <tr><td><b>Part I</b></td><td>Raul Guarini Riva (<a href="https://epge-classes.github.io/econometrics-fgv-2026/">Part I Website</a>)</td></tr>
  <tr><td><b>TA</b></td><td>Taric Latif (<a href="mailto:tariclatif@gmail.com">tariclatif@gmail.com</a>)</td></tr>
  <tr><td><b>Classes</b></td><td>Wednesdays and Fridays, 9:00–11:00 (20 hours · 10 sessions)</td></tr>
  <tr><td><b>Syllabus</b></td><td><a href="syllabus/Syllabus_Econometrics_and_Causal_Inference_EPGE_2026.pdf">Syllabus (PDF)</a></td></tr>
  <tr><td><b>Lecture Notes</b></td><td><a href="notes/Econometrics_and_Causal_Inference.pdf">Econometrics and Causal Inference (PDF)</a></td></tr>
</table>

## Learning Goals

This course provides an advanced introduction to causal identification strategies in applied economic research, starting from causal questions, well-defined estimands, and explicit identification assumptions before turning to estimation, inference, diagnostics, and robustness.

By the end of the course, you should be able to:

- Formulate well-defined causal estimands for economic and policy questions;
- State and justify the assumptions required for causal identification;
- Compare experimental and quasi-experimental research designs;
- Interpret how treatment-effect heterogeneity shapes common econometric estimators;
- Critically evaluate the internal credibility and external validity of empirical studies.

## Course Units & Schedule

| # | Unit & Main Topics | Hours |
|---|---|---|
| 1 | **Potential Outcomes, Causal Estimands, and Identification** — Potential outcomes; ATE and ATT; selection bias; effect heterogeneity; good and bad controls | 2h30 |
| 2 | **Randomized Experiments and Selection on Observables** — Randomization; inference and balance; regression adjustment; propensity score, IPW, AIPW, and matching | 2h30 |
| 3 | **Instrumental Variables and LATE** — Instrument validity; first stage; Wald and 2SLS; compliers and LATE; weak instruments | 3h00 |
| 4 | **Regression Discontinuity Designs** — Sharp and fuzzy RD; local polynomial estimation; bandwidth choice; bias correction; manipulation and diagnostic tests | 2h30 |
| 5 | **Difference-in-Differences: Foundations** — Two-group/two-period setup; parallel trends; event studies; inference and serial correlation | 2h00 |
| 6 | **Modern Difference-in-Differences and Event Studies** — Staggered adoption; TWFE limitations; Goodman–Bacon decomposition; group-time ATT; modern event studies | 3h00 |
| 7 | **Synthetic Control and Comparative Case Studies** — Synthetic control construction; donor pool; pre-treatment fit; placebos; extensions and links to DiD | 2h00 |
| 8 | **Diagnostics, Sensitivity Analysis, Robustness, and Research Design** — Identification robustness; placebos; sensitivity analysis; cluster inference; external validity; design audit | 2h30 |

## Materials

The primary reference is the course monograph, organized around the eight units above:

- Pinho Neto, V. R. (2026). [*Econometrics and Causal Inference*](notes/Econometrics_and_Causal_Inference.pdf). Graduate Lecture Notes, FGV EPGE.

Complementary textbooks:

- Angrist, J. D., & Pischke, J.-S. (2009). *Mostly Harmless Econometrics: An Empiricist's Companion*. Princeton University Press.
- Imbens, G. W., & Rubin, D. B. (2015). *Causal Inference for Statistics, Social, and Biomedical Sciences*. Cambridge University Press.
- Cunningham, S. (2021). *Causal Inference: The Mixtape*. Yale University Press.
- Hernán, M. A., & Robins, J. M. (2020). *Causal Inference: What If*. Chapman & Hall/CRC.

## Evaluation (Part II)

| Weight | Component | Description |
|---|---|---|
| **80%** | Exam | Written evaluation of the theoretical and methodological content of the course |
| **10%** | Problem-set quiz | Quiz based on the problem sets, with one question randomly drawn from the assigned problems |
| **10%** | Empirical exercise | Group empirical assignment applying methods studied in the course |

## Problem Sets

There are four consolidated problem sets (each covering two course chapters), posted under [`problem_sets`](problem_sets):

- **Problem Set 1** (*Potential Outcomes, Randomized Experiments, and Selection on Observables* — Chapters 1–2): [PDF](problem_sets/PS1/problem_set_01.pdf) · [Data: `job_training.csv`](problem_sets/PS1/job_training.csv)  
  *Due Wednesday, December 2, 2026 (deliver in class).*
- **Problem Set 2** (*Instrumental Variables and Regression Discontinuity Designs* — Chapters 3–4): *coming soon*
- **Problem Set 3** (*Difference-in-Differences and Event Studies* — Chapters 5–6): *coming soon*
- **Problem Set 4** (*Synthetic Control, Diagnostics, and Research Design* — Chapters 7–8): *coming soon*

## Publishing to GitHub Pages

1. Push this repository to GitHub (e.g., under `epge-classes`).
2. In **Settings → Pages**, set **Build and deployment → Source** to **GitHub Actions**.
3. Pushing to `main` automatically deploys the course webpage via [`.github/workflows/pages.yml`](.github/workflows/pages.yml).

To release a new problem set:
1. Place its PDF (and any dataset) in `problem_sets/PSN/`.
2. In `index.html`, replace that row's `<span class="soon">coming soon</span>` with a `<span class="links">...</span>` block modeled on PS1/PS2.

## License

Course materials are licensed under [CC BY 4.0](LICENSE).
