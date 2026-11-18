# From Risk Factors to Risk Signals

Code for the Master thesis "From Risk Factors to Risk Signals: A Text-Based Analysis of Geopolitical Risk Disclosure in 10-K Filings". The notebooks extract Item 1A (Risk Factors) from the 10-K filings of S&P 1500 firms for fiscal years 2018–2025 (10,962 firm-years, 1,488 firms), measure geopolitical risk disclosure with a lexicon-based NLP pipeline, validate the measures against LLM labels and the Caldara–Iacoviello GPR index, and estimate the models reported in the thesis. The notebooks are stored with the executed outputs reported in the thesis.

## Pipeline

1. `notebooks/00_CIK_Matcher.ipynb`: SEC CIKs for the S&P 1500 constituents.
2. `notebooks/01_Item1A_Scraper.ipynb`: 10-K retrieval from EDGAR and Item 1A extraction.
3. `notebooks/03_Data_inspection.ipynb`: structural integrity and text-quality checks.
4. `notebooks/05_NLP_pipeline.ipynb`: geo-sentence classification, indicators, novelty measures, LLM validation sample.
5. `notebooks/04_Financials_scraper.ipynb`: WRDS data and analysis panel (Sections 11–12 use the output of 05).
6. `notebooks/06_Regressions.ipynb`: intensity, composition, interaction, filing-window and predictive models.
7. `notebooks/06b_Identification.ipynb`: variance decomposition, exposure event study, long differences, GPR timing.
8. `notebooks/07_External_Validation.ipynb`: benchmark against the Caldara–Iacoviello GPR index.

## Thesis tables and figures

| Thesis | Notebook, section | File in `results/` |
|---|---|---|
| Table 3 | 06, Section 9 | `table_03.csv` |
| Table 4 | 05, Section 8 | `table_04.txt` |
| Table 5 | 05, Section 8 | `table_05.txt` |
| Table 6 | 06, Section 9 | `table_06.csv` |
| Table 7 | 06, Section 9 | `table_07.txt` |
| Table 8 | 06, Section 3A | `table_08.csv` |
| Table 9 | 06b, Sections 3a and 3b | `table_09_panel_a.csv`, `table_09_panel_b.csv`, `table_09_panel_b_groups.csv` |
| Table 10 | 06, Section 9 | `table_10.csv`, `table_10_tone_negative_only.csv` |
| Table 11 | 06, Section 9 | `table_11_effects.csv`, `table_11_differences.csv` |
| Table 12 | 06, Section 9 | `table_12.csv` |
| Table 13 | 06, Section 9 | `table_13.csv` |
| Table 14 | 06, Section 9 | `table_14.csv` |
| Figure 1 | 07, Section 4 | `figure_01.png` |
| Figure 2 | 06b, Section 3a | `figure_02.png` (panels A and B) |
| Table III.1 | 05, lexicon cell | `appendix_table_III_1.csv`; full lists in `data/lexicons/lexicons.csv` |
| Appendix VII | – | `prompts/validation_prompt_v2.md` |
| Appendix VIII | 05, Section 10 | `appendix_VIII_precision_recall.csv` |
| Appendix IX | 05, Section 10 | `appendix_IX_pipeline_vs_majority.csv`, `appendix_IX_between_raters.csv` |
| Appendix X | 04 | – |
| Table VII.1 | 06, Section 9 | `appendix_table_VII_1.csv` |
| Table VIII.1 | 06, Section 9 | `appendix_table_VIII_1.csv` |
| Table VIII.2 | 06, Section 9 | `appendix_table_VIII_2.csv` |
| Table VIII.3 | 06, Section 5 | `appendix_table_VIII_3_autocorrelation.csv`, `appendix_table_VIII_3_persistence.csv` |
| Table VIII.4 | 06, Section 9 | `appendix_table_VIII_4.csv` |
| Table XIII.1 | 06b, Sections 1 and 1b | `appendix_table_XIII_1.csv`, `appendix_table_XIII_1_summary.csv`, `appendix_table_XIII_1_transitory.csv` |
| Table XIII.2 | 06b, Section 3a | `appendix_table_XIII_2.csv` |
| Figure XIII.1 | 06b, Section 3a | `appendix_figure_XIII_1.png` (panel C) |
| Table XIV.1 | 07, Section 6 (fiscal-period rows); 06b, Section 2 (other rows) | `appendix_table_XIV_1_fiscal_period.txt`, `appendix_table_XIV_1_before_filing.csv` |
| Table XIV.2 | 06b, Section 2b | `appendix_table_XIV_2.csv` |

## Data

- SEC EDGAR filings: public; rebuilt by notebooks 00 and 01.
- Compustat, CRSP, I/B/E/S, CRSP–Compustat link table: WRDS subscription required; pulled by notebook 04.
- Caldara–Iacoviello GPR index: download `data_gpr_export.xls` from https://www.matteoiacoviello.com/gpr.htm to `data/validation/external/`.
- `data/SP1500_CIK.csv` (sample firms), `data/lexicons/` (all lexicons), `prompts/` (LLM validation prompt), `output/validation/v2/` (validation sample, packets and rater returns).

## Paths

Notebooks 00, 01 and 03 use paths relative to the repository root (01 reads `SP1500_CIK.csv`, stored as `data/SP1500_CIK.csv`); notebooks 04–07 use paths relative to `notebooks/`. Export file names in `output/tables/` follow working numbers; `results/` uses the thesis numbering.

## Installation

```
pip install -r requirements.txt
python -m spacy download en_core_web_trf
```

Python 3.14 (notebooks 00–03: Python 3.12).

## Citation

Schlißke, S. (2026). From Risk Factors to Risk Signals: A Text-Based Analysis of Geopolitical Risk Disclosure in 10-K Filings. Master's thesis, University of St. Gallen.