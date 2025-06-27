# Project Overview

This repository contains the final working code for this thesis. Please note that the development process involved extensive experimentation and debugging, but only the refined, functional code is presented here for clarity.

## Repository Structure

The codebase is organized into multiple Jupyter notebooks, categorized by research phase and specific topics covered within each phase. You can also find the results (pkl files) in the 'Metrics' folder. Metrics names are self-explanitory, but they also are explained in the following table: 
### Summary of Metric DataFrames

| Metric DataFrame Name                      | Experiment Phase | Model Type             | Data Scope / Filtering               | Input Features          |
| :----------------------------------------- | :--------------- | :--------------------- | :----------------------------------- | :---------------------- |
| `metrics_one4all_10days_raw_NB`            | Initial          | N-BEATS (Multi-series) | First 10 days                        | Raw Input               |
| `metrics_one4all_10days_raw_RNN`           | Initial          | RNN (Multi-series)     | First 10 days                        | Raw Input               |
| `metrics_one4all_10days_raw_filteredmoneyness_NB` | Initial          | N-BEATS (Multi-series) | First 10 days, Filtered by Moneyness | Raw Input               |
| `metrics_one4all_10days_raw_filteredmoneyness_RNN` | Initial          | RNN (Multi-series)     | First 10 days, Filtered by Moneyness | Raw Input               |
| `metrics_df_all_per_symbol_raw`            | Initial          | N-BEATS(Model-per-symbol)       | All symbols, 28 days                 | Raw Input               |
| `metrics_df_one4all_goodsymbols_raw_NB`    | Main             | N-BEATS (Multi-series) | Filtered symbols                     | Raw Input               |
| `metrics_df_one4all_goodsymbols_raw_RNN`   | Main             | RNN (Multi-series)     | Filtered symbols                     | Raw Input               |
| `metrics_df_one4all_goodsymbols_allfeatures_NB` | Main             | N-BEATS (Multi-series) | Filtered symbols                     | All Features  |
| `metrics_df_one4all_goodsymbols_allfeatures_RNN` | Main             | RNN (Multi-series)     | Filtered symbols                     | All Features  |

## Data Availability

The experiments is fully reproducible if the necessary data is available. However, the complete options datasets used in this project is **not included** in this repository because it was purchased from Tardis.dev on a per-person basis. For more information about the license, please see [https://tardis.dev/#pricing](https://tardis.dev/#pricing) and contact my ING supervisor.

If similar data is purchased and downloaded, the provided code can be used to fully reproduce all processing steps and experiments. The results of different experiments in the 'Metrics' folder are available, and the notebooks related to analyzing these metrics are fully reproducible. (Please ensure you update the folder path, typically found at the beginning of the notebooks).
