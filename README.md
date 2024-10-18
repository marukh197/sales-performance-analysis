
# Sales-Performance-Analysis
Flask API for sales performance analysis, generating feedback on individual and team metrics using GPT-2. Includes endpoints for rep performance, team summary, and performance trends forecasting.

## Setup and Installation

### Prerequisites:

Before running this project, ensure you have the following installed:
- Python 3.x
- Anaconda or any other Python virtual environment manager
- Flask
- pandas
- transformers (Hugging Face pipeline)
- TensorFlow (for managing verbosity settings)


### Installation Steps:

1. Clone the repository: git clone https://github.com/marukh197/sales-performance-analysis
  	

2. Navigate to the project directory: cd sales-performance-api
	

3. Create and activate a virtual environment:   conda create --name sales_api_env python=3.8
						conda activate sales_api_env

4.Install the required dependencies:  pip install -r requirements.txt

5. Place the sales_performance_data.csv file in the project directory.				
-----------------------------------------------------------------------------------
Alternatively, you can manually install the packages:

pip install Flask pandas transformers tensorflow


## How to Run

1.open jupyter-notebook
2.run app.ipynb
3.application will start on http://127.0.0.1:3500 (you can change the port)


## API Endpoints

### 1. Individual Sales Representative Performance

URL: /api/rep_performance
Method: GET
Query Parameters: rep_id( The employee ID of the sales representative.)
example: http://127.0.0.1:3400/api/rep_performance?rep_id=183


### 2. Team Performance Summary

URL: /api/team_performance
Method: GET
example: http://127.0.0.1:3400/api/team_performance


### 3. Performance Trends and Forecasting

URL: /api/performance_trends
Method: GET
Query Parameters:
time_period: Either monthly or quarterly.
example: http://127.0.0.1:3300/api/performance_trends?time_period=monthly


## Technologies Used

Flask
pandas
Hugging Face Transformers: Used for the GPT-2 text generation model for generating feedback and forecasts.
TensorFlow: Included for logging and managing verbosity.















