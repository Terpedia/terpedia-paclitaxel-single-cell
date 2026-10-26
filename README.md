# Paclitaxel single-cell exposure analysis

A compact, descriptive analysis of [GEO GSE266934](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE266934): HCC1143 cells exposed to 1 nM paclitaxel or 0.1% DMSO for 24 or 72 hours. Paclitaxel is a taxane diterpenoid. This is chemical-exposure single-cell RNA-seq, not genetic Perturb-seq.

- [Executed Jupyter notebook](notebooks/terputer-paclitaxel-single-cell.ipynb)
- [Generated evidence brief](research/paclitaxel-single-cell/generated/white-paper.md)
- [Analysis script and methods](research/transcriptomics/gse266934/README.md)
- [Results and figure](research/transcriptomics/gse266934/results)

Run with Python dependencies from `requirements.txt`:

```sh
python notebook-runner.py notebooks/terputer-paclitaxel-single-cell.ipynb . 300 '["research/transcriptomics/gse266934/results/library_qc.tsv","research/transcriptomics/gse266934/results/module_contrasts.tsv","research/transcriptomics/gse266934/results/marker_cpm_ratios.tsv"]'
node report-generator.mjs research/transcriptomics/gse266934/report-spec.json
```

The source archive is downloaded and SHA-256 verified. The notebook runner records a receipt matching the saved notebook and the result files written during that run. The version 2 report specification requires those hashes for observed claims. There is one library per condition, so these comparisons are descriptive and do not establish biological reproducibility or target dependence.
