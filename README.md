# aiml

Hands-on notebooks for core machine learning ideas (Stanford ML Specialization–style labs), using Python, NumPy, and pandas—meant for **learning**, not production pipelines.

## Environment

Python **3.13+**. Install dependencies:

```bash
uv sync
```

Use Jupyter, VS Code, or Cursor with the interpreter where this project’s packages are installed (`ipykernel` is included for notebooks).

## Suggested learning order

| Order | Notebook | What you practice |
|------:|----------|-------------------|
| 1 | [`src/linear_regression/linear_regression.ipynb`](src/linear_regression/linear_regression.ipynb) | One feature, cost, gradient descent, normalization |
| 2 | [`src/linear_regression/vectorization.ipynb`](src/linear_regression/vectorization.ipynb) | NumPy vectorization habits |
| 3 | [`src/linear_regression/multiple_linear_regression.ipynb`](src/linear_regression/multiple_linear_regression.ipynb) | Several features, matrix \(X\), gradients in multiple dimensions |

Other topics (e.g. RAG) live under `src/` as separate tracks.

## Data

Place datasets under `datasets/`. Notebooks under `src/linear_regression/` load CSV files with paths like `../../datasets/...`—keep that layout or update the paths in the first code cells.

## Tips while you learn

- **Run top-to-bottom** after edits; old variables (`X_train`, `w`, `\alpha`) are a common source of “impossible” errors.
- **Feature scale:** If gradient descent blows up (`inf`, `nan`), normalize inputs and/or reduce the learning rate `\alpha`.
- **Symbols:** Markdown in the notebooks matches the equations—\(m\) examples, \(n\) features, \(\mathbf{x}^{(i)}\) as one row.

---

*Companion practice for Stanford — ML Specialization.*
