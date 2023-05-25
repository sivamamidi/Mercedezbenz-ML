# Mercedes Benz Dataset Analysis

This repository contains code to analyze the Mercedes Benz dataset using Python and pandas. The code performs various data preprocessing and feature engineering techniques, including data type analysis, handling high cardinality, and count frequency encoding.

## Dataset

The dataset used in this analysis is `mercedesbenz.csv`, which contains information about various features of Mercedes Benz cars.

## Code Explanation

1. Loading the Dataset:
   - The dataset is loaded using the `pd.read_csv()` function and stored in a DataFrame called `df`.
   - The initial structure of the DataFrame is displayed using `df.head()`.

2. Data Type Analysis:
   - The `data_type()` function is defined to analyze the data types of the features in the DataFrame.
   - It counts the number of integer, float, object, and other data types.
   - The summary of data types is printed, providing an overview of the data.

3. Distinct Categories Analysis:
   - The `distinct_categories()` function is defined to analyze the number of unique categories in each object feature of the DataFrame.
   - It prints the number of categories and the value counts for each object feature.

4. Handling High Cardinality - Count Frequency Encoder:
   - The code implements count frequency encoding to handle high cardinality in object features.
   - The `count_frequency_encoder()` function identifies the top categories with the highest occurrences for each object feature.
   - It applies one-hot encoding on these categories, creating new binary columns for each selected category.
   - The original object features are dropped from the DataFrame.
   - The function returns the modified DataFrame with count frequency encoded features.

5. Encoding Features based on Percentage Threshold:
   - The `encoding_features()` function encodes object features based on a given percentage threshold.
   - It selects the top categories that constitute a specified percentage (n%) of the data.
   - One-hot encoding is applied to these categories, and new binary columns are created.
   - The original object features are dropped from the DataFrame.
   - The function returns the modified DataFrame with encoded features.

## Usage

1. Clone the Repository:

2. Install Dependencies:
- Make sure you have Python and pandas installed.
- You can install the required dependencies using pip:
  ```
  pip install pandas
  ```

3. Run the Code:
- Open the cloned repository in your preferred Python environment.
- Run the code in a Python script or Jupyter Notebook.
- Modify the code as needed for your specific use case.

Feel free to explore and adapt the code to suit your requirements. Enjoy analyzing the Mercedes Benz dataset!


