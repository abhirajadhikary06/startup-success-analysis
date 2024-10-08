# Startup Success Prediction Project

## Overview

The **Startup Success Prediction Project** aims to predict the success of startups based on key features such as total funding, funding rounds, and startup age. We utilize machine learning algorithms and an interactive dashboard for visualizing insights.

## Installation

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/abhirajadhikary06/startup-success-analysis.git
   cd startup-success-prediction
2. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
## Dataset

The dataset was obtained from Crunchbase via [Kaggle](https://www.kaggle.com/datasets/yanmaksi/big-startup-secsees-fail-dataset-from-crunchbase). The dataset contains several key features including:

-   **category_list**: Industry category of the startup.
-   **funding_total_usd**: Total funding amount in USD.
-   **funding_rounds**: Number of funding rounds the startup has gone through.
-   **founded_at**: Date the startup was founded.
-   **first_funding_at**: Date the startup received its first funding.
-   **last_funding_at**: Date the startup received its last funding.
-   **startup_age**: Age of the startup.
-   **time_to_first_funding**: Time (in months) taken to get the first funding.
    ```bash
    https://www.kaggle.com/datasets/yanmaksi/big-startup-secsees-fail-dataset-from-crunchbase
   ##  Data Preprocessing
To ensure the data is ready for analysis, we handled missing values and cleaned the dataset:

1.  **Handled Missing Values**: Replaced missing values in `funding_total_usd` with the mean of the column and filled missing categorical values (e.g., `category_list`, `country_code`) with the mode.
2.  **Date Conversion**: Converted date columns (like `founded_at`, `first_funding_at`, and `last_funding_at`) into ordinal format for ease of analysis in machine learning models.   
## Exploratory Data Analysis

### **Key Insights:**

-   **Funding Distribution by Industry**: Box plots were created to show how different industries vary in total funding.
-   **Startup Age vs Funding**: Scatter plots were used to explore relationships between startup age and total funding.
-   **Correlation Analysis**: A heatmap visualized the correlation between key variables such as total funding, startup age, and funding rounds.
## **Machine Learning Model**

### **Logistic Regression for Startup Success Prediction**

We implemented a Logistic Regression model to predict whether a startup will succeed based on several features:

-   **Independent Variables**: funding_total_usd, funding_rounds, founded_at, first_funding_at, last_funding_at, startup_age, etc.
-   **Model Performance**: The model's accuracy was evaluated using a confusion matrix and classification report.
## **Visualization Dashboard**

We built an interactive dashboard using Dash and Plotly to present key insights from the analysis.

-   **Funding Distribution by Industry**: A box plot showing the distribution of funding across various industries.
-   **Correlation Heatmap**: Displays the correlations between variables like total funding, startup age, and funding rounds.
-   **Scatter Plot**: Visualizes the relationship between startup age and success.
## **Results**

-   The **Logistic Regression** model yielded promising results with an accuracy of **98%**.
-   The **visual dashboard** provided insightful visualizations of startup success factors, helping users interactively explore the data.
 ## **How to Run**

1.  Clone the repository and navigate to the project directory.
2.  Install the required dependencies using `pip install -r requirements.txt`.
3.  Run the dashboard by executing `python app.py`.
4.  Visit `http://127.0.0.1:8050/` in your web browser to interact with the dashboard.
## Future Work

-   Explore additional machine learning models like Random Forest or SVM for improving prediction accuracy.
-   Include more features such as team size, founder experience, and geographic factors.
-   Expand the dashboard with more advanced visualizations, filters, and predictive capabilities.
-   Google Drive Link : [Startup-Success-Analysis](https://drive.google.com/drive/folders/1l3YFj57CHDhu7KAvSCeIQk2RrufWzxdY?usp=sharing)
## Contributing

Feel free to submit issues or pull requests. All contributions are welcome!
## License

This project is licensed under the MIT License - see the LICENSE file for details.
