# Grocery-Store-Capstone-Project
⏳ Grocery-Store-Forecasting-Challenge-For-Azubian
python fastapi Open Source Love png1

📂 Dataset and Definitions
Main variable definitions

Target: the total sales for a product category at a particular store at a given date

Stores_id: the unique store id

Category_id: the unique Product category id

Date: date in numerical representation

Onpromotion: gives the total number of items in a Product category that were being promoted at a store at a given date

Nbr_of_transactions: the total number of transactions happened at a store at a given date

year_weekofyear: the combination of the year and the week of the year, (year_weekofyear = year*100+week_of_year

ID: the unique identifier for each row in the testing set: year_week_{year_weekofyear}{store_id}{Category_id}

The dataset used is the Grocery sales,public dataset. This is anonymised real data. The data looks at 54 different stores in the same country and 33 different products. The train set contains transaction information for 3 years and 6 months. You are tasked with forecasting the next 8 weeks for the same stores and same products. In this case the series is not stationary with some small seasonalities which change every year.

In order to obtain a exact copy of the dataset used in this tutorial please run the script in which you will get acess to download the dataset.

📚 Analysis and transforms
Time series decomposition

Level
Trend
Seasonality
Noise
Stationarity

AC and PAC plots
Rolling mean and std
Dickey-Fuller test
Making our time series stationary

Difference transform
Log scale
Smoothing
Moving average
📐 Models tested
Randomforest Link
Nearest neighbors Link
XGBoost Link
DecisionTree [Link](https://scikit-learn.org/stable/modules/tree.html
Autoregression (AR)
Seasonal autoregressive integrated moving average (SARIMA)
Autoregressive integraded moving average (ARIMA)
Evaluation Metrics
Root Mean Squared Error (RMSE)
Model	RMSE
Randomforest	64.12
Decision Tree	55.89
XGBOOST	41.41
KNN	49.93
AR	206.0
SARIMA	196.49
ARIMA	191.14
Project Description
This project combines machine learning and FastAPI to develop a powerful and scalable application for predictive analytics and real-time data processing."

Table of Contents
Overview Of the Project
Description of dataset
Application / Deployed Links

Technology Stack

Deliverables

Installation

Execution

API Endpoints

App Usage

Contributing Instructions

Collaborators

Contact Information

1. Overview Of the Project
i. Description of dataset
2. Application / Deployed Links
App	Deployed links
Streamlit App	Sales forecasring App with streamlit
Api	Sales forecasring App with FastAPI
3. Technology Stack
Technology	Version
Python	3.9
Sckit-learn	0.24.1
XGboost	1.7.3
FastAPI	0.98.0
Streamlit	1.23.1
Uvicorn	0.22.0
4. Deliverables
A jupyter notebook for training a classification model
A sales forecasting Model
An API App built with FastApi
A Streamlit app that make calls to the build and hosted API
A Dockerfile for easy deployment
5. Installation
Clone the repository to your local machine:

    git clone https://github.com/kwasiasomani/Grocery-Store-Forecasting-Challenge-For-Azubian.git
Navigate to the project directory:

    cd Grocery-Store-Forecasting-Challenge-For-Azubian
Create a new virtual environment and activate the virtual:

Windows:

  python -m venv venv; venv\Scripts\activate; python -m pip install -q --upgrade pip; python -m pip install -qr requirements.txt  
Linux & MacOs:

  python3 -m venv venv; source venv/bin/activate; python -m pip install -q --upgrade pip; python -m pip install -qr requirements.txt
Execution
Notebooks To run any the notebooks:
Navigate the project folder on anaconda terminal root :: Grocery-Store-Forecasting-Challenge-For-Azubian> ...
Run the command 'jupyter notebook'
Navigate to the notebook '.....ipynb'
Run cells in the notebook
API
To execute the API, follow these steps: After all requirement have been install

At the root of your repository in your terminal root :: Grocery-Store-Forecasting-Challenge-For-Azubian> ... run the command:

        uvicorn src.api.api:app --reload 
OR

        python src/api/api.py
Open your browser and go to http://127.0.0.1:8000/docs to access the API documentation

App
To execute the app, follow these steps: After all requirement have been install

At the root of your repository in your terminal root :: Grocery-Store-Forecasting-Challenge-For-Azubian> ... run the command:

        streamlit run src\app\app.py
Open your browser and go to http://localhost:8501

7. Power BI Visualization
 visualization.mp4 
8. Contributing Instructions
To contribute to the Sentiment Analysis API, follow these guidelines:

Fork the repository.
Create a new branch: git checkout -b my-new-feature
Make your changes and commit them: git commit -am 'Add some feature'
Push to the branch: git push origin my-new-feature
Create a new pull request
9. Collaborators
Name
Bright Eshun
Kwasi Asomani
Stella Oiro
Linda Azdigbli
Foster Kwabena Abrefa
Joshua
10. Contact Information
Name	Twitter	LinkedIn	GitHub	Hugging Face
Bright Eshun	@bright_eshun_	@brighteshun	@bright136	@bright1
Contributing
Do you have anything to add or fix? I'll be happy to talk about it! Open an issue/PR :)
