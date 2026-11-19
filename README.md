# The Cost of Remittance from Singapore, 2011–2025

A data-analytics study by Caleb Teo of what it costs migrant workers to send money home from Singapore, and how policy can better support them. It analyses 230,652 cleaned price quotes from the World Bank's Remittance Prices Worldwide survey across 354 in-scope corridors, joined with seven other datasets, to answer three questions: how the cost of sending USD 200 has moved against the UN SDG 10.c targets, how much of the price is fee versus foreign-exchange margin, and which corridor characteristics are associated with lower costs.

This was made as a module project for NUS High's CS4132, Data Analytics, built August–October 2026 in Python (pandas, statsmodels, scikit-learn, matplotlib, seaborn, plotly). The lecturer, Mrs Phylliscia Lee, graded the project A+:

> "A strong and ambitious project with clear research questions, thoughtful analysis, clear and well planned visualizations."

## Repository layout

| Path | Contents |
|---|---|
| `ProjectReport_CalebT.ipynb` | The full report: data acquisition, cleaning, analysis, findings and recommendations |
| `Appendix_CalebT.ipynb` | Appendix A (evidence trail for every number quoted in the report), Appendix B (model tournament framework) and Appendix C (AI use declaration) |

## Findings in brief

- The cost of sending USD 200 from Singapore fell by about half over 2011–2025 and has plateaued since 2022 above the 3% SDG target; all nine Singapore corridors meet the 5% ceiling on the UN's three-cheapest-services measure.
- The fall came from the visible fee. The FX margin rose only slightly, so its share of the price doubled.
- Worldwide, a corridor's bank share of quotes is the strongest factor associated with higher cost; corridors with larger remittance outflows and diasporas are cheaper.

## Running the notebooks

The datasets are not redistributed here. Download them from their sources into a `data/` folder next to the notebooks, using these file names:

| File in `data/` | Source |
|---|---|
| `1_rpw_dataset_2011_2025_q1.xlsx` | [World Bank, Remittance Prices Worldwide](https://remittanceprices.worldbank.org/data-download) |
| `2_Bilateralremittancematrix2018Oct2019.xlsx` | [World Bank, Bilateral Remittance Matrix 2018](https://thedocs.worldbank.org/en/doc/904591573826885707-0090022019/original/Bilateralremittancematrix2018Oct2019.xlsx) |
| `3_migration_imputed_2024.csv` | [UNU-CRIS Annual Bilateral Migration Database (RIKS), 2024 release](https://data.mendeley.com/datasets/cpt3nh6jct/2) |
| `4_MCI_data_2026.xlsx` | [GSMA Mobile Connectivity Index](https://www.mobileconnectivityindex.com/index.html#year=2025&dataSet=indexScore) |
| `5_API_BX.TRF.PWKR.DT.GD.ZS_DS2_en_excel_v2_33456.xls` | [World Bank WDI, personal remittances received (% of GDP)](https://data.worldbank.org/indicator/BX.TRF.PWKR.DT.GD.ZS) |
| `6_undesa_pd_2024_ims_stock_by_sex_destination_and_origin.xlsx` | [UN DESA, International Migrant Stock 2024](https://www.un.org/development/desa/pd/content/international-migrant-stock) |
| `7_HDR25_Composite_indices_complete_time_series.csv` | [UNDP, Human Development Report 2025 data](https://hdr.undp.org/data-center/documentation-and-downloads) |
| `8_API_FP.CPI.TOTL.ZG_DS2_en_excel_v2_375483.xls` | [World Bank WDI, inflation, consumer prices (annual %)](https://data.worldbank.org/indicator/FP.CPI.TOTL.ZG) |

Then run `ProjectReport_CalebT.ipynb` from top to bottom, followed by `Appendix_CalebT.ipynb` (the appendix re-runs the report and reads its saved outputs, so keep both in the same folder). Besides the usual scientific Python stack, the report needs `joypy`, `plotly`, `xlrd` and `openpyxl`.

The interactive map (Figure 17) does not render in GitHub's notebook preview; open the notebook in Jupyter to see it.

## License

**Copyright © 2026 Caleb Teo. All rights reserved.**

The report, code and figures in this repository are made available for viewing and reference only, and may be cited with attribution. No permission is granted to copy, modify, merge, publish, distribute, sublicense, or sell any part of this repository without the prior written permission of the copyright holder. The underlying datasets belong to their respective publishers and are subject to their own terms.
