# Paclitaxel single-cell exposure analysis

A compact, descriptive analysis of [GEO GSE266934](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE266934): HCC1143 cells exposed to 1 nM paclitaxel or 0.1% DMSO for 24 or 72 hours. Paclitaxel is a taxane diterpenoid. This is chemical-exposure single-cell RNA-seq, not genetic Perturb-seq.

- [Executed Jupyter notebook](notebooks/terputer-paclitaxel-single-cell.ipynb)
- [Generated evidence brief](research/paclitaxel-single-cell/generated/white-paper.md)
- [Analysis script and methods](research/transcriptomics/gse266934/README.md)
- [Results and figure](research/transcriptomics/gse266934/results)

Run with Python dependencies from `requirements.txt`:

```sh
python research/transcriptomics/gse266934/analysis.py
node report-generator.mjs research/transcriptomics/gse266934/report-spec.json
```

The source archive is downloaded and SHA-256 verified. There is one library per condition, so these comparisons are descriptive and do not establish biological reproducibility or target dependence.
