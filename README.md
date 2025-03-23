# IBID-CCT
This is the repository for the IPM 2025 paper "IBID-CCT: A Novel Model for Interdisciplinary Breakthrough Innovation Detection based on Cusp Catastrophe Theory"
## Overview
Detecting interdisciplinary breakthrough innovations is critical for identifying scientific advances and fostering original innovation. Previous studies primarily focus on single-dimensional publication characteristics, such as reference-based or citation-based metrics, which fail to fully capture the complexity of interdisciplinary breakthrough innovations. This study introduces the IBID-CCT model (interdisciplinary breakthrough innovation detection based on cusp catastrophe theory) to address this gap. We explain the mechanism of interdisciplinary breakthrough innovation and propose metrics based on interdisciplinary knowledge integration, fusion, and diffusion stages, grounded in IBID-CCT. First, we construct an experimental dataset comprising papers from prestigious academic awards, including the Nobel Prize, Wolf Prize, Crafoord Prize, Breakthrough Prize, and Turing Award. Using this dataset, we train machine learning and deep learning models based on IBID-CCT metrics to identify interdisciplinary breakthroughs. The experimental results show that the IBID-CCT model built on LGBM and the one built on BERT achieve the best results with an F1 score of 0.8631 and 0.8604, respectively. To further analyze the impact of each metric in IBID-CCT, SHAP analysis is applied to interpret the LGBM model’s results, while word distribution and sentiment analysis are used to interpret the BERT model’s outputs. These analyses reveal that interdisciplinary breakthrough innovations typically involve the integration of cutting-edge, diverse knowledge; experience long-term knowledge diffusion; and consistently positively drive multi-field development. Finally, comparative experiments confirm that our IBID-CCT model significantly outperforms existing methods such as the Disruption Index, Reference Interdisciplinarity, and Citation Interdisciplinarity in both breakthrough innovation detection and interdisciplinary breakthrough innovation detection tasks. This research provides a comprehensive framework for understanding the mechanisms of interdisciplinary breakthrough innovations, designing effective models for their detection, and forecasting future trends in innovation.

## Research Overview
The following is the model of this paper. This figure provides an overview of the interdisciplinary breakthrough innovation generation process.
![fig1-model](img/fig1-model.png)

## Directory Tree
```
IBID-CCT                            Root directory
├─ code                             The directory where the running code is stored.
│  ├─ all.ipynb                     The code for training and evaluating the BERT model with all metrics.
│  ├─ all                           The "all" directory is used for input and output in all.ipynb.
│  │  ├─ test.csv                   The test dataset
│  │  ├─ train.csv                  The train dataset
│  │  └─ val.csv                    The val dataset
|  |
│  ├─ all-roberta.ipynb             The code for training and evaluating the RoBERTa model with all metrics.
│  ├─ all_robert                    The "all_robert" directory is used for input and output in all_robert.ipynb.
|  |
│  ├─ all_scibert.ipynb             The code for training and evaluating the SciBERT model with all metrics.
│  ├─ all_scibert                   The "all_scibert" directory is used for input and output in all_scibert.ipynb.
|  |
│  ├─ no_ex.ipynb                   The code for training and evaluating the BERT model with the metrics excluding Halo effect.
│  ├─ no_ex                         The "no_ex" directory is used for input and output in no_ex.ipynb.
|  |
│  ├─ no_ex_robert.ipynb            The code for training and evaluating the RoBERTa model with the metrics excluding Halo effect.
│  ├─ no_ex_rebert                  The "no_ex_rebert" directory is used for input and output in no_ex_rebert.ipynb.
|  |
│  ├─ no_ex_scibert.ipynb           The code for train and evaluating the SciBERT model with the metrics excluding Halo effect.
│  ├─ no_ex_scibert                 The "no_ex_scibert" directory is used for input and output in no_ex_scibert.ipynb.
|  |
│  ├─ only_text.ipynb               The code for train and evaluating the BERT model with text-only metrics.
│  ├─ only_text                     The "only_text" directory is used for input and output in only_text.ipynb.
|  |
│  ├─ only_text_roberta.ipynb       The code for train and evaluating the RoBERTa model with text-only metrics.
│  ├─ only_text_robert              The "only_text_robert" directory is used for input and output in only_text_robert.ipynb.
|  |
│  ├─ only_text_scibert.ipynb       The code for train and evaluating the SciBERT model with text-only metrics.
│  ├─ only_text_scibert             The "only_text_scibert" directory is used for input and output in only_text_scibert.ipynb.
│  └─ forbert.xlsx                  The current forbert.xlsx is the same as ../dataset/forbert.xlsx
|
├─ dataset
│  └─ forbert.xlsx                  forbert.xlsx is the original dataset.
|
├─ img
│  └─ fig1-model.png
|
└─ README.md

```

## Citation
Please cite the following paper if you use these codes and datasets in your work.
```
@article{WANG2025104121,  
               title={{IBID-CCT}: A novel model for interdisciplinary breakthrough innovation detection based on the cusp catastrophe theory},  
               author = {Zhongyi Wang and Na Wang and Haoxuan Zhang and Zeren Wang and Zhou Wang and Junhua Ding and Haihua Chen},  
               journal={Information Processing & Management},  
               volume={62},  
               number={4},  
               pages={104121},  
               year={2025},  
               issn={0306-4573},  
               doi={https://doi.org/10.1016/j.ipm.2025.104121}  
}
``` 
