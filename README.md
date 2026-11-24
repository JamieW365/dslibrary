# dslibrary

A personal data science knowledge library: a collection of self-contained mini-projects, mostly in Jupyter Notebooks, backed by a reusable and installable Python package of helper functions and classes.

It has two purposes:

- **Reference:** a place to revisit methods, code patterns and lessons learned across the data science toolkit.
- **Portfolio:** a showcase of practical skills across the full data science lifecycle, from data engineering through to deployment.

## Contents

Each mini-project has its own README covering the problem, methodology, results and learning outcomes.

| Area | Project | Summary | Key techniques |
|------|---------|---------|----------------|
| Data Engineering & Prep | _coming soon_ | | |
| EDA & Statistics | _coming soon_ | | |
| Supervised Learning | _coming soon_ | | |
| Unsupervised Learning | _coming soon_ | | |
| Time Series | _coming soon_ | | |
| NLP | _coming soon_ | | |
| Vision & Audio | _coming soon_ | | |
| Recommenders | _coming soon_ | | |
| Graphs | _coming soon_ | | |
| Optimization & RL | _coming soon_ | | |
| MLOps & Deployment | _coming soon_ | | |

## Repository structure

```
dslibrary/
├── README.md          # This file: overview and master contents table
├── pyproject.toml     # Packaging configuration
├── data/              # Local data (raw/interim/processed are gitignored)
├── src/dslibrary/     # Installable helper library
├── tests/             # Unit tests for the library
├── docs/templates/    # README and notebook templates for new projects
└── notebooks/         # Mini-projects, grouped by area
    ├── data_engineering_and_prep/
    ├── eda_and_stats/
    ├── supervised_learning/
    ├── unsupervised_learning/
    ├── timeseries/
    ├── nlp/
    ├── vision_and_audio/
    ├── recommenders/
    ├── graphs/
    ├── optimization_and_rl/
    └── mlops_and_deployment/
```

Each project folder under `notebooks/` is self-contained: its own README, numbered notebooks, and any small sample data or assets it needs.

## The `dslibrary` package

Helper functions and classes that prove reusable in the notebooks are moved into `src/dslibrary/`, tested, and imported back into the notebooks.

| Module | Purpose |
|--------|---------|
| `data_engineering` | Loaders, cleaning, pipelines |
| `eda` | Plotting and statistical helpers |
| `supervised` | Model wrappers, cross-validation, metrics |
| `unsupervised` | Clustering and dimensionality reduction |
| `timeseries` | Feature creation, splits, forecasting utilities |
| `nlp` | Tokenisation, embeddings, evaluation |
| `vision_audio` | Transforms and augmentation |
| `recommenders` | Similarity measures and ranking metrics |
| `graphs` | Graph construction and centrality helpers |
| `optimization` | Solvers and RL environments/agents |
| `mlops` | Experiment tracking, serving and config helpers |
| `utils` | Logging, paths, seeding, configuration |

### Installing in another project

Core install:

```bash
pip install "git+https://github.com/<your-username>/dslibrary.git"
```

With optional extras for heavier dependencies:

```bash
pip install "dslibrary[nlp,vision,graphs] @ git+https://github.com/<your-username>/dslibrary.git"
```

## Getting started

```bash
git clone https://github.com/<your-username>/dslibrary.git
cd dslibrary

python3 -m venv .venv
source .venv/bin/activate

pip install -e ".[dev]"
```

Then open a notebook with JupyterLab:

```bash
jupyter lab
```

Individual projects may list extra requirements in their own README or `requirements.txt`.

## Tools

An index of common data science tools and the projects that use them. Rows fill in as projects are added.

| Category | Tool | Projects |
|----------|------|----------|
| Experiment tracking & registry | MLflow | _coming soon_ |
| Experiment tracking & registry | Weights & Biases | _coming soon_ |
| Cloud storage | AWS S3 | _coming soon_ |
| Data warehousing | Amazon Redshift | _coming soon_ |
| Data warehousing | BigQuery | _coming soon_ |
| Data processing | Apache Spark / PySpark | _coming soon_ |
| Data processing | dbt | _coming soon_ |
| Workflow orchestration | Apache Airflow | _coming soon_ |
| Pre-trained models & datasets | Hugging Face | _coming soon_ |
| Deep learning | PyTorch | _coming soon_ |
| Deep learning | TensorFlow / Keras | _coming soon_ |
| Classical ML | scikit-learn | _coming soon_ |
| Gradient boosting | XGBoost / LightGBM | _coming soon_ |
| Model serving & APIs | FastAPI | _coming soon_ |
| Containerisation | Docker | _coming soon_ |
| Vector search | FAISS | _coming soon_ |
| Graph analysis | NetworkX | _coming soon_ |
| Optimization | OR-Tools / PuLP | _coming soon_ |

## Licence

Released under the [MIT Licence](LICENSE).