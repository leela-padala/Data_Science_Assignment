# Data Science Assignment

Python notebooks maintained by **Leela Padala**, covering exploratory analysis, data integration, and visualization. These are supporting data-analysis exercises, not security detection systems.

## Notebook Guide

| Notebook | Implemented work | Data requirement |
| --- | --- | --- |
| [Student Performance Analysis](Student_Performance_Analysis.ipynb) | Score distribution and grouped boxplots for reading, writing, and math | Upload the included `StudentsPerformance.csv` |
| [Data Integration and Visualization](Week2_DataIntegrationAndVisulaization_(1).ipynb) | Merge/join, concatenation, filtering, grouped summaries, and matplotlib/Plotly charts | Internet access to the external datasets referenced in the notebook |
| [Frailty and Grip Strength](Copy_of_Frailty_Grip_Strength.ipynb) | Missing-value checks, binary frailty encoding, correlation, and boxplot | `frailty_data.csv`, available in [Frailty_Analysis](https://github.com/leela-padala/Frailty_Analysis/blob/main/frailty_data.csv) |

## Running the Exercises

Open the selected notebook in Google Colab. Student Performance and Frailty use `google.colab.files` to request an upload. Use the exact filenames expected by the code. The integration notebook additionally uses Plotly and downloads datasets over the network.

For the frailty notebook, start with the initialization/analysis cell in a fresh runtime; its first cell refers to a dataframe that has not yet been created. Original notebook code is preserved.

## Interpretation and Limitations

- Student charts show associations within the supplied dataset. They do not demonstrate that lunch category, parental education, gender, or test preparation causes a score difference.
- Frailty uses a ten-record sample and is not suitable for clinical conclusions.
- The integration exercise includes a derived `Cases` field summing confirmed, recovered, and death counts. These overlap and must not be interpreted as unique infection counts.
- External datasets may change or become unavailable. There is no pinned data snapshot or automated regression suite.
- Saved outputs demonstrate prior notebook activity, not a guarantee that every cell runs unchanged in a new environment.

## Validation

The documentation review checked notebook JSON structure, code dependencies, CSV headers, and repository links. It did not claim fresh end-to-end execution. For a new run, verify row counts after joins, missing values, category mappings, and chart labels before interpreting outputs.

## Sources and Attribution

External data references include [M3IT COVID-19 Data](https://github.com/M3IT/COVID-19_Data) and [datasets/covid-19](https://github.com/datasets/covid-19). Existing notebook references to pandas documentation and datagy.io are retained. The source of `StudentsPerformance.csv` has not been independently verified during this documentation update.
