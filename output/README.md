# Description of `output` subdirectory

This subdirectory contains the output for our Strong Baseline and the two extensions. This contains data on both the dev and test data. You can load this data and use the function `read_csv` to evaluate it on the .ipynb notebook as well.
The easiest way we would recommend doing this is to just run the .ipynb notebook from start to end so that you won't have to download or upload any output files for evaluation. Both the model and evaluation scripts are already contained in the notebook.

Below, we also provide samples of the metrics we used for evaluation. 

# Model Evaluation Results

- **Test Accuracy**: 0.49925


## Simple Baseline

### Dev. Classification Performance:

| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| CG    | 0.00      | 0.00   | 0.00     | 2003    |
| OR    | 0.50      | 1.00   | 0.67     | 1997    |
| Accuracy    | -     | -   | 0.50     | 4000    |
| Macro Avg    | 0.25      | 0.50   | 0.33     | 4000    |
| Weighted Avg    | 0.25      | 0.50   | 0.33     | 4000    |

## Strong Baseline

### Test Confusion Matrix
|  |  |
|-------|-----------|
| 1884    | 137      | 
 83    | 1896     |

- **Test Accuracy**: 94.50%
- **Test Precision**: 93.26%
- **Test Recall**: 95.81%

### Test Classification Performance:

| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| CG    | 0.96      | 0.92   | 0.94     | 2003    |
| OR    | 0.93      | 0.96   | 0.94     | 1997    |
| Accuracy    | -     | -   | 0.94     | 4000    |
| Macro Avg    | 0.95      | 0.95   | 0.94     | 4000    |
| Weighted Avg    | 0.95      | 0.94   | 0.94     | 4000    |

---
