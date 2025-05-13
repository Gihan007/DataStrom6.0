
# Insurance Agent Performance Prediction & Improvement

### Overview

This project focuses on predicting and improving the performance of insurance agents by leveraging real-world data provided by ABC Insurance Company. The primary goals are to identify agents at risk of not selling policies ("NILL") and to recommend personalized performance improvement plans for existing agents.

### Problem Statement

* **Part 1: Predict NILL Agents**

  * Forecast which agents are at risk of failing to make sales in the following month (i.e., "One Month NILL").
  * Identify the key factors influencing early agent performance.
  * Suggest personalized SMART action plans for at-risk agents (e.g., training, mentoring).

* **Part 2: Monitor and Improve Existing Agent Performance**

  * Track current agent performance over time.
  * Categorize agents into High, Medium, and Low performers.
  * Recommend interventions based on performance categories.
  * Track progress over time and evaluate the effectiveness of interventions.

### Dataset

The dataset provided contains historical agent performance data, including:

* **Agent Information**: agent age, join date, first policy sold date, etc.
* **Performance Metrics**: proposals, quotations, customers, new policies sold, and other features.

### Tools & Libraries Used

* **Programming Language**: Python
* **Libraries**: pandas, numpy, matplotlib, seaborn, scikit-learn, statsmodels
* **Frameworks**: Jupyter Notebooks for EDA, Streamlit for dashboard/visualization (optional)

### Project Structure

1. **EDA.ipynb**: Exploratory Data Analysis (EDA) with insights and visualizations.
2. **datastrom\_EDE.ipynb**: This notebook contains all the steps for performing the exploratory data analysis and generating insights from the dataset.
3. **new\_model.ipynb**: This notebook contains the model training process for predicting NILL agents and categorizing agents based on their performance.
4. **README.md**: This file.

### Steps to Run the Project

#### 1. Clone the Repository

```bash
git clone https://github.com/username/repository.git
cd repository
```

#### 2. Install Dependencies

Install the required Python libraries using the following command:

```bash
pip install -r requirements.txt
```

#### 3. Perform Exploratory Data Analysis (EDA)

* Run the `datastrom_EDE.ipynb` notebook to perform the following tasks:

  * **Key Metrics & Distributions**: Summary statistics and visualizations.
  * **Sales Patterns**: Analysis of how sales patterns vary by month and identification of any unexpected trends.
  * **Multivariate Analysis**: Exploring relationships between numerical features using correlation matrices and pair plots.
  * **Agent Trajectories**: Analyzing the performance evolution of individual agents over time.
  * **Innovative EDA**: Advanced insights, including outlier detection, feature engineering, and transformations.

#### 4. Train the Model (Part 1)

* Run the `new_model.ipynb` notebook to build and train the prediction model for **One Month NILL** using the following steps:

  * **Preprocessing**: Handle missing data, outliers, and feature transformations (Box-Cox, Min-Max scaling, PCA, etc.).
  * **Model Selection**: Train models like KNN or any other suitable algorithms to predict at-risk agents.
  * **Evaluate Model**: Evaluate the accuracy and performance of the model using appropriate metrics like F1-score, Precision, Recall, or AUC.

#### 5. Categorize Agents and Recommend Interventions (Part 2)

* Implement the agent performance categorization logic (Low, Medium, High) based on features like `new_policy_count`, `net_income`, and `number_of_policy_holders`.
* For each performance category, recommend personalized interventions such as:

  * **Low Performers**: Targeted training and mentoring.
  * **Medium Performers**: Coaching and motivational strategies.
  * **High Performers**: Recognition and reward systems.

#### 6. Dashboard (Optional)

* If a dashboard is built, use Streamlit or another tool to visualize:

  * Agent classification results.
  * Performance tracking over time.
  * Suggested interventions for each group.
  * Model predictions for at-risk agents.

### Key Metrics & Evaluation Criteria

The project will be evaluated based on the following criteria:

* **EDA (15 points)**: Insightfulness of data exploration and the quality of charts and explanations.
* **Accuracy of NILL Prediction Model (25 points)**: Performance of the model in predicting agents at risk of going "NILL."
* **Insightfulness of Influencing Factors (10 points)**: Identification of the key factors influencing agent performance.
* **Personalized Action Plans (15 points)**: Quality and relevance of the action plans suggested for at-risk agents.
* **Effectiveness of Classification Logic (15 points)**: Proper categorization of agents into performance tiers (Low, Medium, High).
* **Intervention Strategy (10 points)**: Thoughtfulness of the proposed interventions for agents based on their performance category.
* **Dashboard or Visualization (10 points)**: Creation of a useful dashboard or visualizations for monitoring agent performance.

### Final Deliverables

1. **Code Files or Notebooks**: All Jupyter notebooks used for EDA and model training.
2. **Trained Models**: The model used for predicting "NILL" agents, or instructions on how to train it.
3. **Visualizations**: All charts, plots, and any dashboards built to show predictions and agent classifications.
4. **README**: A clear explanation of your approach, intervention logic, and insights.

### License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


