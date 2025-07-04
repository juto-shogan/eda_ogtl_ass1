
# Customer Support Case Analysis Dashboard

## Overview

This project delivers a comprehensive analysis of customer support cases, providing key insights into support operations, common customer issues, and performance trends. It encompasses a detailed Exploratory Data Analysis (EDA) conducted in a **Jupyter Notebook** (`eda.ipynb`) and culminates in an interactive **Streamlit dashboard** (`app.py`). The dashboard allows for dynamic filtering and visualization of case data, enabling stakeholders to quickly identify patterns, monitor key metrics, and make informed decisions to improve customer service efficiency and satisfaction.

## Key Questions / Objectives

* **Case Status Overview:** Understand the distribution of customer support cases by their current status (e.g., open, closed, pending).
* **Customer Segmentation Analysis:** Analyze cases based on various customer segments and subsegments to identify specific needs or issues per customer group.
* **Product Line Impact:** Determine the volume and nature of cases related to different product lines.
* **Top Reasons for Contact:** Identify the most frequent top-level and sub-level reasons why customers contact support.
* **Monthly Trend of Cases:** Track the temporal evolution of customer support cases to detect trends, seasonality, or anomalies over time.
* **Interactive Data Exploration:** Provide a user-friendly interface for dynamic filtering and visualization of the case data.

## Dataset

* **Name:** Customer Support Cases
* **Source:** The primary dataset for this analysis is `data/data.csv`.
* **Description:** This dataset contains records of customer support interactions, including information such as 'Opened Date', 'Status', 'Customer Segmentation', 'Customer Subsegmentation', 'Product Line', 'Top-Level Reason', and 'Sub-Reason'. It is pre-processed to handle missing values and duplicates to ensure data quality for analysis.

## Project Structure

| File Name            | Description                                                                                                                                                                       |
| :------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `eda.ipynb`        | The primary Jupyter Notebook for in-depth Exploratory Data Analysis (EDA). It covers data loading, cleaning, preliminary analysis, and static visualizations.                     |
| `app.py`           | The Python script that powers the interactive Streamlit web application. It loads the processed data, generates dynamic charts, and provides filtering options for the dashboard. |
| `data/data.csv`    | The raw dataset containing all customer support case records.                                                                                                                     |
| `requirements.txt` | Lists all Python libraries and their exact versions required to run the project successfully.                                                                                     |
| `README.md`        | This README file, providing an overview, setup instructions, and details about the project.                                                                                       |

## Technologies / Libraries Used

* **Python 3.x**
* **Pandas:** Essential for robust data loading, manipulation, and cleaning operations.
* **NumPy:** For efficient numerical computations, often used implicitly by Pandas.
* **Matplotlib:** For foundational plotting capabilities, especially during initial EDA.
* **Seaborn:** Used for creating aesthetically pleasing statistical graphics, enhancing visualization quality.
* **Plotly Express & Plotly Graph Objects:** Utilized extensively for generating interactive, web-based data visualizations within both the Jupyter Notebook and the Streamlit dashboard.
* **Streamlit:** The framework chosen for building the interactive and user-friendly web dashboard, making the analytical insights accessible to a broader audience.

## Setup and Installation

1. **Clone the Repository**

   ```bash
   git clone [https://github.com/juto-shogan/customer-support-analysis.git](https://github.com/juto-shogan/customer-support-analysis.git)
   cd customer-support-analysis
   ```

   *(Remember to replace `customer-support-analysis.git` with your actual repository name if different)*
2. **Create a Virtual Environment (Recommended)**

   ```bash
   python -m venv venv
   # On Windows:
   # .\venv\Scripts\activate
   # On macOS/Linux:
   # source venv/bin/activate
   ```
3. **Install Dependencies**

   ```bash
   pip install -r requirements.txt
   ```

## How to Run the Analysis & Dashboard

1. **Activate your virtual environment** (if created):

   * On Windows: `.\venv\Scripts\activate`
   * On macOS/Linux: `source venv/bin/activate`
2. **Explore the Jupyter Notebook (`eda.ipynb`):**
   To understand the detailed data preparation, exploratory data analysis steps, and initial static visualizations:

   ```bash
   jupyter notebook eda.ipynb
   ```

   This command will open the Jupyter environment in your web browser, allowing you to execute cells and follow the analytical workflow.
3. **Run the Interactive Dashboard (`app.py`):**
   To launch the interactive Streamlit dashboard and dynamically explore the customer support case insights:

   ```bash
   streamlit run app.py
   ```

   This command will open the dashboard in your default web browser, typically at `http://localhost:8501`.

## Findings / Insights

* **Dominant Case Reasons:** Preliminary analysis indicates that "Others" and "Queries" are frequently reported top-level reasons for customer contact, suggesting a need for more granular categorization to pinpoint specific issues.
* **Customer Segmentation Impact:** Cases vary significantly across different customer segments and subsegments, indicating that tailored support strategies might be beneficial.
* **Monthly Case Volume Fluctuations:** The monthly trend of cases reveals notable fluctuations, which could be influenced by seasonal factors, product launches, or marketing activities. Further investigation into these periods can provide actionable insights.
* **Product-Specific Issues:** Certain product lines generate a higher volume of support cases, highlighting areas that may require product development or documentation improvements.
* [**YOUR INSIGHT HERE**: Add any other specific, compelling insights you uncovered during your analysis, such as "Identified a spike in cases related to 'Billing' immediately after a service update," or "Customers in segment X consistently report issues with feature Y."]

## Author

Somto Mbonu

Data Analyst
GitHub Profile: [juto-shogan](https://github.com/juto-shogan)
