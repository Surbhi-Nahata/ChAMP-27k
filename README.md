# CHAMP methylation array workflows

This workspace keeps the HumanMethylation27 and Methylation Screening Array (MSA) analyses in separate folders. The pipelines use platform-matched manifests and annotations; do not mix their IDATs, manifests, or probe filters.

## Workflows

- [`27k_champ/`](27k_champ/README.md) contains the HumanMethylation27 workflow documentation and sample-sheet template for GSE68319 / GPL8490.
- [`msa_champ/`](msa_champ/README.md) contains a separate MSA workflow for selected IDAT samples from GSE264438 / GPL34394, including its notebook and metadata templates.

## Data handling

Raw GEO IDAT files and generated results are excluded from Git. Each workflow downloads only the samples configured in its sample sheet; do not download or commit the full GEO archive unless needed.

The current workspace did not contain the previously described 27K notebook/code, only the 27K README and sample-sheet template. Those materials have been copied into `27k_champ/`; the MSA work is isolated in `msa_champ/`.
