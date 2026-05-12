# Digital Facilitation Impact Analysis

Repository per l'analisi d'impatto degli interventi di facilitazione digitale attraverso:

- survey ai fruitori del servizio
- eventuali dataset esterni
- analisi statistiche
- visualizzazioni dei risultati

---

# Struttura del progetto

```text
digital-facilitation-impact-analysis/
│
├── README.md
├── pyproject.toml
├── poetry.lock
├── .gitignore
│
├── config/
│   └── settings.yaml
│
├── data/
│   ├── raw/
│   ├── interim/
│   ├── processed/
│   └── external/
│
├── notebooks/
│
├── outputs/
│   ├── figures/
│   ├── tables/
│   └── reports/
│
├── src/
│   ├── main.py
│   │
│   ├── ingestion/
│   │   └── load_data.py
│   │
│   ├── processing/
│   │   ├── clean_survey.py
│   │   └── feature_engineering.py
│   │
│   ├── analysis/
│   │   ├── descriptive_analysis.py
│   │   ├── impact_analysis.py
│   │   └── statistical_tests.py
│   │
│   ├── plotting/
│   │   └── plots.py
│   │
│   └── utils/
│       ├── io.py
│       └── logger.py
│
└── tests/
    └── test_processing.py
```

---

# Setup ambiente

## Installazione Poetry

### Linux / macOS

```bash
curl -sSL https://install.python-poetry.org | python3 -
```

### Verifica installazione

```bash
poetry --version
```

---

## Installazione ambiente

```bash
poetry install
```

## Attivazione ambiente

```bash
source $(poetry env info -p)/bin/activate
```
