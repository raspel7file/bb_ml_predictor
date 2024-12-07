# Blood Bowl 3 Official Ladder Results Predictor
## Goals and Objectives
1. Create ML-model, which can predict the result of "Blood Bowl 3" Official Ladder match. Predictors should be simple and available in game at the moment of a match start.
2. Achieve better results, than random predicting.
3. Present results to audience as a piece of software.
4. Ruin goblins-bookmakers!

## Stack
- Python 3.12.4 (pandas, CatBoost, sklearn, optuna, gradio)  
- Analytic Workspace BI System  
- bits of HTML, CSS, JavaScript only with AI help

## Workflow
First, we had to get data, using Cyanide API. Details are [here](https://github.com/raspel7file/bb_data_extractor).

Second, training ML model on this data (see ladder_predictions.ipynb in this repository).

Third, raise an app, which does the job of predicting [here](https://huggingface.co/spaces/raspel/BB_predictions).

Fourth, visualize results at AW BI (well, it's technically a dashboard, but works as an app interface) [here](https://aw-demo.ru/public/dashboard/DCrmUvVip-0IzdocOJbLoItBTiGog61j)

## Results
- Model for predicting BB3 Ladder results is created, works with roughly 50% accuracy (1.5 times better than random predicting).  
- It has drawbacks, but it is a good start.  
- You can try to predict your match result [here](https://aw-demo.ru/public/dashboard/DCrmUvVip-0IzdocOJbLoItBTiGog61j)
