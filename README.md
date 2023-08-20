# Predicting solar irradiance using satellite images

This product aims to provide ground irradiance estimation at Synergy Technology Co., Ltd. by using a cloud attenuation model that takes cloud cover index extracted from Himawari-8 satellite as an input.
<p align="center">
  <img src="https://github.com/NuttamonThungka/Predict_irradiance/assets/113121308/3dc3441f-f308-4e45-b666-9ae9fa957884" width="800" height="400" />
</p>

This repository is composed of the following folders
- **trainning** are utilized for downloading data, cleaning it, and generating datasets. And contains training code for the models. There are 5 model: linear regression, polynomial regression, randomforest, XGBoost and CNN model.
- **Implementation** is used for implement code with contain app to deploy the deshboard.
## Web app

[Predicting solar irradiance using satellite images](https://predirr-ixgmley8iuerkfnbm9ap4t.streamlit.app/)
<p align="center">
  <img src="https://github.com/NuttamonThungka/Predict_irradiance/assets/113121308/844f631a-2840-4d1a-95fb-5134eef8038a" width="900" height="500" />
</p>

## Deploy in local host
1. Clone git : ```git clone https://github.com/NuttamonThungka/Pred_irr.git```
2. Create a new conda environment : ```conda create -n pred_irr```
3. Activate the conda : ```conda activate pred_irr```
4. Go to the folder Pred_irr : ```cd <path to folder>```
5. Install the requirments to run the app.py ```pip install -r requirements.txt```
6. Run the ```app.py``` with using streamlit : ```streamlit run app.py```


## Deploy in streamlit web
1. Create git hub repository and upload 5 files to deploy the web application in streamlit.
- ```app.py``` is the python code to run the web application
- ```Synergy_testset.csv``` is the input of the model to generate the predicted irradiance
- ```RandomForest.joblib``` is the propesed model usinf random forest model
- ```compare_model_result.csv``` is the result data of each trained model
- ```requirements.txt``` is the requirements of the module version that use in this project

2. go to [streamlit web](https://streamlit.io/) and sign in/ log in (you can also connect with your git hub)
3. In streamlit website :
   - 3.1 you go to click ```New app```
   - 3.2 selected repository with includ 5 files in 1.
   - 3.3 Branch : ```main```
   - 3.4 Main file app : ```app.py```
   - 3.5 click : ```Deploy```


