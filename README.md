#  Customer Subscription Prediction using Decision Tree

This project builds a **Decision Tree Classifier** to predict whether a customer will subscribe to a **term deposit** based on their **demographic and behavioral data**. The model is trained on the **Bank Marketing Dataset** provided by the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing).



##  Project Overview

In this project, we aim to:
- Understand customer data collected through marketing campaigns
- Build a supervised machine learning model using a decision tree
- Evaluate its performance in predicting customer subscription behavior
- Visualize how the model makes decisions



##  Dataset Description

The dataset contains information on direct marketing campaigns conducted by a Portuguese bank, where the goal was to promote term deposit subscriptions.

**Source:** [UCI Machine Learning Repository – Bank Marketing Dataset](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing)

### Files Used:
| File Name         | Description                                   |
|-------------------|---------------------------------------------  |
| `bank.csv`        | A smaller, sampled version with 4,521 records |
| `bank-full.csv`   | The complete dataset with 45,211 records      |

### Key Features:
- `age`: Age of the client
- `job`: Type of job (e.g., admin., technician)
- `marital`: Marital status
- `education`: Education level
- `contact`: Contact communication type
- `month`, `day_of_week`: Last contact date
- `duration`: Last contact duration in seconds
- `campaign`: Number of contacts during the campaign
- `pdays`, `previous`: Past campaign contact information
- `y`: **Target variable** – whether the client subscribed (`yes` or `no`)



##  Model Used

A **Decision Tree Classifier** from `scikit-learn` is used because:
- It is interpretable and easy to visualize
- It handles both numerical and categorical data well
- It works well for classification tasks like this one



##  Tools & Libraries

- Python
- Jupyter Notebook
- `pandas`, `numpy` for data handling
- `sklearn` for model training and evaluation
- `matplotlib` for visualization



##  Project Workflow

1. **Data Loading**
   - Read `bank.csv` and `bank-full.csv` using pandas.
   
2. **Preprocessing**
   - Handled categorical variables using one-hot encoding.
   - Split the data into features (`X`) and target (`y`).
   - Performed train-test split.

3. **Model Training**
   - Trained a Decision Tree model using `criterion='entropy'`.

4. **Evaluation**
   - Evaluated using:
     - Accuracy Score
     - Classification Report
     - Confusion Matrix

5. **Visualization**
   - Visualized the trained tree using `plot_tree()`.



##  Results

Both datasets (`bank.csv` and `bank-full.csv`) were used and compared. Key observations:
- `bank.csv` allows quick experimentation.
- `bank-full.csv` provides better generalization with more data.

The model outputs include:
- Tree structure visualization
- Accuracy and classification performance
- Confusion matrix insights



##  Key Learnings

- Gained experience in data preprocessing and feature encoding
- Learned how decision trees classify data based on entropy
- Understood how dataset size and quality affect model performance
- Practiced visualizing and interpreting machine learning models








