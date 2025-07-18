# Credit-Risk-Probability-Model
An End-to-End Implementation for Building, Deploying, and Automating a Credit Risk Model

## Credit Scoring Business Understanding.
1. How does the Basel II Accord’s emphasis on risk measurement influence our need for an interpretable and well-documented model?
- Basel II puts a strong focus on how banks measure and manage risk, so our model needs to be both transparent and explainable. If regulators or internal teams can’t understand how it works, they won’t trust the results no matter how accurate it is.

2. Since we lack a direct "default" label, why is creating a proxy variable necessary, and what are the potential business risks of making predictions based on this proxy?
- Without a clear default label, we need a proxy to train the model. It’s not ideal, but it gives us a way to move forward. The risk is that if the proxy doesn’t closely match actual defaults, we might misclassify customers either rejecting good ones or approving risky ones.

3. What are the key trade-offs between using a simple, interpretable model (like Logistic Regression with WoE) versus a complex, high-performance model (like Gradient Boosting) in a regulated financial context?
- Simple models are easier to explain and defend to regulators, even if they sacrifice some accuracy. Complex models may perform better but can be a black box, which raises concerns around fairness, transparency, and compliance. It’s a balance between performance and trust.

## Project Directory Structure

The repository is organized into the following directories:

`.github/workflows/`: Contains configurations for GitHub Actions, enabling continuous integration and automated testing.

`api`: Contains the implementation of the machine learning model API, allowing interaction with the model through RESTful endpoints.

`notebooks/`: Jupyter notebooks used for tasks such as data exploration, feature engineering, and preliminary modeling.

`scripts/`: Python scripts for data preprocessing, feature extraction, and the implementation of the credit scoring model.

`tests/`: Unit tests to ensure the correctness and robustness of the implemented model and data processing logic.



## Installation Instructions

To run the project locally, follow these steps:

1. Clone the Repository:
>>>>
    git clone https://github.com/korerima/Credit-Risk-Probability-Model.git`

    cd Credit-Risk-Probability-Model
>>>>

2. Set up the Virtual Environment:

Create a virtual environment to manage the project's dependencies:

**For Linux/MacOS**

>>>
    python3 -m venv .venv

    source .venv/bin/activate  
>>>

**For Windows:**

>>>
    python -m venv .venv
    .venv\Scripts\activate
>>>

3. Install Dependencies:

Install the required Python packages by running:
>>>
    pip install -r requirements.txt
>>>
