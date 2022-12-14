# nucleoside-finder

This repository contains a Jupyter Notebook used to search Orbitrap LC-MS/MS data for nucleosides. This notebook was written by [Peter Thuy-Boun](https://github.com/petertb), with additions by [Adair Borges](https://github.com/borgesadair1). 

## Inputs: 
This repo contains mass lists for nucleosides, charged adducts, and neutral adducts as inputs to the script: `mass_list_charged_adducts.csv`, `mass_list_neutral_adducts.csv`, `mass_list_nucleosides.csv`. Orbitrap data analyzed here are available through Zenodo: [10.5281/zenodo.7319990](https://zenodo.org/record/7319990#.Y4UDYuxuewk)

## Outputs: 
We have included the outputs from the script: `dRibose_neutral_loss_combined_raw_results.csv` contains raw results from this analysis, and `dRibose_neutral_loss_scatter.jpg` is a scatterplot of precursor ion m/z to fragment m/z. `dRibose_neutral_loss_summary_results.csv` is the most useful file with the nicely summarized results. 

## Development 
This software was developed and tested on Apple M1 macOS Monterey v12.1. To run the notebook, install the packages listed in the `env.yml` file using `conda`.
You can find operating system-specific instructions for installing miniconda [here](https://docs.conda.io/en/latest/miniconda.html).
After installing conda and [mamba](https://mamba.readthedocs.io/en/latest/), run the following command to create the environment.

```
mamba env create -n jupyter_nbs --file env.yml
conda activate jupyter_nbs
```

Once you have the environment activated, you can start a jupyter instance using:
```
jupyter notebook
```
