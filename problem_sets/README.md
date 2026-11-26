# Problem Sets — Econometrics and Causal Inference (FGV EPGE 2026)

Numbered references to tables, figures, equations, sections, and results in the problem sets refer to the [Lecture Notes](../notes/Econometrics_and_Causal_Inference.pdf).

## Problem Set 1 — Potential Outcomes, Randomized Experiments, and Selection on Observables (Chapters 1–2)

- **Due date:** Wednesday, December 2, 2026 (deliver in class)
- **PDF:** [`PS1/problem_set_01.pdf`](PS1/problem_set_01.pdf)
- **Data:** [`PS1/job_training.csv`](PS1/job_training.csv)

### Codebook: `job_training.csv` (Problem Set 1, Problem 10)

2,935 workers: participants in a job-training program (`sample = program`), an experimental control group (`experimental_control`), and a comparison group from a national household survey (`survey`). Comma-separated with variable names in the first row.

| Variable | Description |
|---|---|
| `id` | Worker identifier |
| `sample` | `program`, `experimental_control`, or `survey` |
| `treat` | 1 if the worker participated in the program; 0 otherwise |
| `age` | Age in years |
| `educ` | Years of schooling |
| `black`, `hisp` | 1 if Black; 1 if Hispanic |
| `married` | 1 if married |
| `nodegree` | 1 if no high-school degree |
| `re74`, `re75` | Earnings in 1974 and 1975 (before the program), US dollars |
| `re78` | Earnings in 1978 (after the program), US dollars |
