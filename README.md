# SLOTH (Single-cell Lineage on Targeted Hypermutation)

<p align="center">
  <img src="docs/SLOTH.gif?raw=true" alt="SLOTH" title="SLOTH" width="200" height="200">
</p>

---

[![GitHub](https://img.shields.io/github/license/mashape/apistatus.svg)](/LICENSE.md)
[![DOI:10.1038/s41592-021-01325-x](https://zenodo.org/badge/DOI/10.1038/s41592-021-01325-x.svg)](https://doi.org/10.1038/s41592-021-01325-x)
[![Citation Badge](https://api.juleskreuer.eu/citation-badge.php?doi=10.1038/s41592-021-01325-x)](https://www.nature.com/articles/s41592-021-01325-x/metrics)


Mapping single-cell-resolution cell phylogeny reveals cell population dynamics during organ developments

## PROCEDURE

- **Single Molecule Sequecing Pipeline** ([smrt](./smrt))

  - Adaptors Trimming
  - Circular Consensus Sequence Generation
  - Align to Reference Sequence
  - Annotate Sequence Features
  - Link Sample Barcode Sequence
  - Cluster Molecular Indentifier (UMI) Sequence
  - Group Reads by Sample Barcode and Molecular Indentifier
  - Generate Consensus Sequence for Lineage Barcode
  - Call Mutation
  - Post Quality Filter

- **Single Cell Tree Construction** ([tree](./tree))

  - Build Tree by Maximum Likelihood Method
  - Fix Tree
  - Visualize Tree

- **Benchmarking Cell Lineage Tracing System** ([benchmark](./benchmark))

  - `alemany_whole-organism_2018`
  - `bowling_engineered_2020`
  - `chan_molecular_2019`
  - `chen_efficient_2020`
  - `kalhor_developmental_2018`
  - `lee-six_population_2018`
  - `mckenna_whole-organism_2016`
  - `pei_polylox_2017`
  - `quinn_single-cell_2021`
  - `raj_simultaneous_2018`
  - `spanjaard_simultaneous_2018`

- **Simulation** ([simu](./simu))

  - Generate Cell Tree (division / differentiation / mutation)
  - Subsample Barcoded Cells
  - Reconstruct Cell Lineage Tree

- **Population Dynamics** ([pop](./pop))

  - ?

## READ MORE

scientific question :
https://celllineage.github.io/SLOTH/index.html

technical details:
https://github.com/CellLineage/SLOTH/wiki

## HOW TO USE?

```bash
git clone https://github.com/CellLineage/SLOTH.git
```

---

## CITATION

Liu, K., Deng, S., Ye, C. et al. Mapping single-cell-resolution cell phylogeny reveals cell population dynamics during organ development. **Nat Methods** 18, 1506–1514 (2021). [https://doi.org/10.1038/s41592-021-01325-x](https://doi.org/10.1038/s41592-021-01325-x)

## LICENSE

The content of this project itself is created by **Ye Chang** and licensed under the [Creative Commons Attribution 4.0 International License (CC BY)](https://creativecommons.org/licenses/by/4.0/),
and the underlying source code used to format and display that content is licensed under the [MIT license](LICENSE.md).

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
