# Graph Neural Network for Remaining Useful Life Prediction Benchmarking [[Paper]()] 


[//]: # (<p align="center">)

[//]: # (<img src="misc/temporal_adapt.PNG" width="900" class="center">)

[//]: # (</p>)

## Requirmenets:
- Python3
- Pytorch==1.10
- Numpy==1.22
- scikit-learn==1.4.1
- Pandas==1.3.5
- skorch==0.15.0 

## Datasets

### Available Datasets
We used four public datasets in this study. We also provide the **preprocessed** versions as follows:
- [C-MAPSS](https://data.nasa.gov/Aerospace/CMAPSS-Jet-Engine-Simulated-Data/ff5v-kuh6/about_data)
- [N-CMAPSS](https://drive.google.com/drive/folders/1231PMXaKEVMfwWzwnjujIUzULdjiYC1c) (No. 17 in thie link)
- [PHM2012](https://github.com/Lucky-Loek/ieee-phm-2012-data-challenge-dataset)
- [XJTU-SY](https://drive.google.com/drive/folders/1_ycmG46PARiykt82ShfnFfyQsaXv3_VK)


### Dataset Preprocess

1. Put the respective data in Data_process/Datasets
2. Process the dataset with its corresponding .py file, i.e., Data_process/Datasets/Data_read_{}.py

### Training a model

To train a model:

```
python main.py  --experiment_description exp1  \
                --run_description run_1 \
                --GNN_method FC_STGNN \
                --dataset CMAPSS \
                --dataset_id FD004 \
                --bearing_id Testing_bearing_1 \ # Need to specify for XJTU_SY
                --num_runs 5 \
```




## Citation
If you found this work useful for you, please consider citing it (paper will be available soon).

[//]: # (```)

[//]: # (@inproceedings{mpau,)

[//]: # (  author = {Ragab, Mohamed and Eldele, Emadeldeen and Foo, Chuan-Sheng and Wu, Min and Li, Xiaoli and Chen, Zhenghua},)

[//]: # (  title = {Source-Free Domain Adaptation with Temporal Imputation for Time Series Data},)

[//]: # (  booktitle={29th SIGKDD Conference on Knowledge Discovery and Data Mining - Research Track},)

[//]: # (  year = {2023},)

[//]: # (  url={https://openreview.net/forum?id=v6GK0ijPW0B})

[//]: # (})

[//]: # (```)


## Acknowledgement

We appreciate the code from [ADATIME](https://github.com/Lucky-Loek/ieee-phm-2012-data-challenge-dataset) and [Dataset link](https://github.com/Lucky-Loek/ieee-phm-2012-data-challenge-dataset)