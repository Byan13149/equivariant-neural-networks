# A3 High Energy Physics Coursework

## Setup

```bash
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

## Running the Notebooks

```bash
jupyter notebook
```

Then open either notebook in the browser:

- `theory_solution.ipynb` — equivariant neural networks and symmetry verification
- `experiment_solution.ipynb` — B meson decay analysis (requires data files, see [Data](#data))

Run all cells top-to-bottom. Figures are saved to `figures/`.

## Viewing the Reports

Pre-built PDFs are in `report/`:

- `report/theory.pdf`
- `report/experiment.pdf`

To rebuild from source (requires a LaTeX distribution):

```bash
cd report
pdflatex theory.tex
pdflatex experiment.tex
```

## Repository Structure

```
├── theory_solution.ipynb       # Theory solutions notebook
├── experiment_solution.ipynb   # Experiment solutions notebook
├── A3_Coursework.pdf           # Coursework assignment brief
├── weights_torch_W.pt          # Pre-trained NN weights (NN1)
├── weights_torch_phi.pt        # Pre-trained NN weights (NN2)
├── report/
│   ├── theory.pdf              # Theory report
│   ├── theory.tex              # Theory report (LaTeX source)
│   ├── experiment.pdf          # Experiment report
│   └── experiment.tex          # Experiment report (LaTeX source)
└── figures/                    # Generated analysis figures
```

#### Use of generative AI
Claude (Anthropic) was used to assist with code development and report writing. All outputs were reviewed and tested by the author, who takes full responsibility for the final submission.