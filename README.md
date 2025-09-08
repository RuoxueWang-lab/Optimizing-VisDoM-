# Optimizing-VisDoM-

## Get datasets
1) **Clone the VisDoM datasets**
```bash
git clone https://github.com/MananSuri27/VisDoM
```
Then you can access the datasets SPIQA, SlideVQA, SciGraphVQA, PaperTab, FetaTab, as well as the eval.py for calculating Word Overlap F1 scores.

## Set up environment
```bash
conda env create -f environment.yml
conda activate <env-name>  
```

## Run the code
The ```visdomrag_baseline.py ``` corresponds to the baseline code. To run the code please fill in your own api keys for gemini if you want to run the baseline.
The ```visdomrag_optimized.py``` combined with ```visdomrag_main.py``` corresponds to the code for experiment V1, if you want to run V1, please change the corresponding configurations inside visdomrag_main.py, and fill in the api keys for the model you want to use. And do ```from visdomrag_optimized import VisDoMRAG, logger``` at the top of the visdomrag_main.py, then run visdomrag_main.py.
The ```visdomrag_optimized_PL.py``` combined with visdomrag_main.py corresponds to the code for experiment V2, if you want to run V1, please change the corresponding configurations inside visdomrag_main.py, and fill in the api keys for the model you want to use. And do ```from visdomrag_optimized_PL import VisDoMRAG, logger``` at the top of the visdomrag_main.py, then run visdomrag_main.py.
