# Helpful Input Files

Some of the preprocessing steps are very time consuming. We decided to output some of the necessary input files that can be run directly without the need to remake them, saving a lot of runtime.

## `code_vocab.json`

The prebuilt file containing the vocabulary for all codes contained in the patient data. Each unique code is mapped to an integer value, which is used by each custom task to convert the codes into a useful format for our BEHRT model.

## `task1_optuna.db`, `task2_optuna.db`, `task3_optuna.db`

Optuna database files containing the history of trials for each hyperparameter tuning process (for Tasks 1, 2, and 3 respectively). These can be used by Optuna to get the best parameters without needing to perform the hyperparameter optimization again.

## Usage

Place all files within Google Drive using the following path:

```python
/content/drive/MyDrive/{the file name}
