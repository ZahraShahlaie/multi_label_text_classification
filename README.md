# multi_label_text_classification
Multi-label text classification


In this project, we want to classify input samples of the Ronash dataset into 20 categories via its title, vendor, and tags. Click on the below link and enjoy!
---

In this notebook, I present the updated version of the multi-label text classification model created by Farakh Karimi. The original model achieved an accuracy of 81.21% and a loss of 0.8373. In the updated version, the following changes have been made to improve the model performance:

### Exploratory Data Analysis (EDA):

- **Distribution of Products by Vendors**
- **Pie Chart of Product Distribution by Category**
- **Histogram of Number of Tags per Product**
- **Bar Plot of the Top 10 Most Frequent Tags**

### Class Balancing:

- Data analysis by grouping based on the 'category' column and counting the number of products in each category (`category_counts = df['category'].value_counts()`).
- Correcting class imbalance using upsampling.

### Improving Text Transformation Layer Parameters:

- Re-defining `max_features` and `sequence_length` parameters:
  - `max_features = 19000` (increased from 10,000 to 19,000)
  - `sequence_length = 320` (reduced from 350 to 320)

### Model Performance Evaluation:

- Improved accuracy and reduced loss:
  - **Loss: 0.1043**
  - **Accuracy: 0.9786**

### Performance Analysis:

- Plotting the confusion matrix and classification report for detailed analysis of the model's performance.

This update demonstrates significant improvements in the performance and stability of the multi-label text classification model.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/farrokhkarimi/multi_label_text_classification/blob/main/multi_label_text_classification.ipynb)
