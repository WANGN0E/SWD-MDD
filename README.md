# SWD-MDD

Reproducible material for **Application of Multi-Dimensional Deconvolution to Enhance Seismic-While-Drilling Data Imaging - Wang N., Ravasi M., Deheuvels M., Alkhalifah T.**

**1produce_data**
- raymckimaging.ipynb:               Calculating input and output (GFs) data for NNs. 
- raymckimaging_ff.ipynb:            Calculating input and output (FFs) data for NNs. 


**2test_data_NN**
- inputdata:          arrange for training, validation and test data: d+ d-
- outputdata:         arrange for training, validation and test data: gf+ gf-
- inputdata_ff:       arrange for training, validation and test data: d+ d-
- outputdata_ff:      arrange for training, validation and test data: ff+ ff-
- create_mask.ipynb:  calculate time mask

**3train_NN_pred**
- main.py :                  The entry point of this project. It coordinates the overall workflow by calling functions from the other sub-programs.
- arrange_data.py:           Since the data is too large, we use this file to arrange for the total data.
- model.py:                  The architecture of the U-Net.
- train.py:                  Training process, validation process and predction process.

**4imaging_ff**
- Image_pred_data_simple.ipynb:    carry out UD-RM imaging

**5produce_sparse_imaging_data**
- simple_sparse.py:    carry out UD-RM imaging for sparse data

## Environment

To ensure reproducibility of the results, we have provided a `environment-latest.yml` file. Ensure to have installed Anaconda
or Miniconda on your computer.

After that simply run:
```
./install_env-latest.sh
```
It will take some time, if at the end you see the word `Done!` on your terminal you are ready to go!



## Cite us 
Wang N. et al. (2025) Application of Multi-Dimensional Deconvolution to Enhance Seismic-While-Drilling Data Imaging. Geophysics.


