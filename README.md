# NovaForge Labs lab results dataset

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.24327269.svg)](https://doi.org/10.5281/zenodo.24327269)

Every certificate of analysis (COA) NovaForge Labs has published, in one machine-readable table.

- **26 lot-specific results** from two independent US laboratories: Freedom Diagnostics (15) and ILS Laboratories (11)
- **HPLC purity:** median 99.78%, range 99.03–99.99%, 20 of 26 at or above 99.5%
- **File:** [`novaforge-lab-results.csv`](novaforge-lab-results.csv)
- **Live version:** https://novaforgelabs.co/lab-results-dataset (updated as new lots are tested)

## Columns

| Column | Meaning |
|---|---|
| `product` | Product name and size as sold |
| `lot_number` | Lot (batch) number as printed in the order confirmation |
| `coa_number` | The laboratory's report ID, for verifying the report with the lab |
| `hplc_purity_percent` | HPLC purity reported by the lab (main-peak share of UV signal) |
| `tested_date` | Test date where printed on the report (blank if not stated) |
| `coa_pdf_url` | Link to the original certificate PDF |

## Methods and limits

- **Freedom Diagnostics** reports confirm identity by LC-MS (observed vs theoretical mass), report HPLC purity, and measure net content in mg.
- **ILS Laboratories** reports confirm identity by HPLC retention-time match against a reference standard and report HPLC purity.
- HPLC purity is not net peptide content: salts, counter-ions and water do not appear in the purity figure. See [HPLC purity vs net peptide content](https://novaforgelabs.co/hplc-purity-vs-net-peptide-content).
- These reports cover identity and purity only. They do **not** include sterility, endotoxin, heavy-metal or residual-solvent testing.
- Results are as reported by the issuing laboratories. Report IDs can be checked with the labs directly.

## License and citation

Released under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). You may share and adapt the data for any purpose with attribution:

> NovaForge Labs (2026). *NovaForge Labs lab results dataset*. Zenodo. https://doi.org/10.5281/zenodo.24327269

All products are sold for laboratory research use only and are not for human or animal consumption.
