
# Fairness Guarantees under Demographic Shift

This repository is the official reproduction of the implementation of [Fairness Guarantees under Demographic Shift](https://openreview.net/pdf?id=wbPObLm6ueA). 

## Requirements

Requires Python 3.x, Numpy 1.16+, and Cython 0.29+

To install further required packages and modules:

```setup
pip install -r requirements.txt
```

The pre-processed datasets, as well as the original datasets, are provided in the repository.

## Training and Evaluation

The experiments from the paper can be executed by running the provided batch file from the Python directory, as follows:

```setup
./iclr_ds_experiments.bat
```
     
Once the experiments are completed, the figures can be generated by running the following batch file.

```setup
./iclr_ds_figures.bat
```
Given that the files are structured as follows:

- results
    - results_original_experiments
        - iclr_adult_{mode}_ds_rl_{constraint}
            - iclr_adult_{mode}_ds_rl_{constraint}.h5
        - iclr_brazil_{mode}_ds_rl_{constraint}
            - iclr_brazil_{mode}_ds_rl_{constraint}.h5
        - etc.
            - etc.
    - results_mlp_experiments
        - etc.
            - etc.
    - results_diabetes_experiments   
        - etc.

Where {mode} can consist of either 'fixed' or 'antag', corresponding to a known and unknown distributional shift respectively, and {constraint} can correspond to 'di' and 'dp', meaning the fairness constraints Disparate Impact and Demographic Parity.

Once completed, the figures will be saved to `Fairness-Guarantees-under-Demographic-Shift/figures/*` by default.


## Experiment results

You can download results of our experiments here:

- [Results](https://drive.google.com/drive/folders/1u41wPeqjdMjkaXf5T0nJtW0i446fycLV?usp=sharing) 

## Overall results

Our model achieves the following performance on :

...

## Contributing

> SeldonianML is released under the MIT license.
