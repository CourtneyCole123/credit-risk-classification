<h1> Module 20 Challenge: Supervised Machine Learning</h1>

<h2>Background</h2>
<p>In this Challenge, you’ll use various techniques to train and evaluate a model based on loan risk. You’ll use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.</p>

<h2>Requirements</h2>

<h3>1. Split the Data into Training and Testing Sets</h3>

- Read the lending_data.csv data from the Resources folder into a Pandas DataFrame.

  ![image](https://github.com/user-attachments/assets/83506953-306c-40f4-bcde-c22f4f3947a4)

- Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.

  ![image](https://github.com/user-attachments/assets/aae5a5c1-c46d-40df-aa87-2167b3cd716d)

- Split the data into training and testing datasets by using train_test_split.

  ![image](https://github.com/user-attachments/assets/4744c9d1-8ea4-4fbe-a103-75b47c5581a9)

<h3>2. Create a Logistic Regression Model</h3>

- Fit a logistic regression model by using the training data (X_train and y_train).

  ![image](https://github.com/user-attachments/assets/ef72e5b8-f5d2-4bae-9fa4-f181eb276ef4)

- Save the predictions on the testing data labels by using the testing feature data (X_test) and the fitted model.

  ![image](https://github.com/user-attachments/assets/b1c631f6-be41-47e6-93e3-4f2e058a8a80)

- Evaluate the model’s performance by doing the following:

  - Generate a confusion matrix.

    ![image](https://github.com/user-attachments/assets/300cf9e7-b7c0-40f5-91ae-358c01c6ebb9)

  - Generate a classification report.

    ![image](https://github.com/user-attachments/assets/8ac547fa-00d1-4e6a-96a9-557eee81d162)

- Answer the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?

  <pre>Answer: The model does a very good job of prdiciting healthy loans with 100% precision. The model is not as adept at predicting hih-risk loans with precision only at 87%. Overall, however, the model's accuracy is 99% which would lead one to believe that it is a good model. </pre>

<h3>3. Write a Credit Risk Analysis Report</h3>

- Provide an overview that explains the purpose of this analysis.

- Using a bulleted list, describe the accuracy, precision, and recall scores of the machine learning model.

- Summarize the results from the machine learning model. Include your justification for recommending the model for use by the company. If you don’t recommend the model, justify your reasoning.

  <pre><h4>Analysis:</h4>
  <p>The objective of this report is to assess the overall creditworthiness of borrowers based on specified criteria. 
    - <strong>Precision:</strong> Precision is defined as the percentage of accurate positive predictions in relation to the total positive predictions. The model successfully predicted high-risk loans for borrowers with an accuracy rate of 87%.
    - <strong>Recall:</strong> Recall is defined as the percentage of accurate positive predictions relative to the total actual positives. For this model, the accuracy rate is 89%.
    - <strong>F1 Score:</strong> The F1 score represents a weighted average of precision and recall, with values closer to 1 indicating better performance. This model achieves an F1 score of 88%, signifying that it functions effectively.
  Given the model's accuracy, I recommend proceeding with its implementation. Additionally, it would be beneficial to continue training the model with more data to enhance its overall accuracy in predicting high-risk borrowers./p>
  
  <h4>Important Note!</h4> I utilized this website to assist me with the definitions for my analysis: https://www.statology.org/sklearn-classification-report/. 
  
  </pre>

<h3>4. Coding Conventions and Formatting</h3>

- Place imports at the top of the file, just after any module comments and docstrings and before module globals and constants.

  ![image](https://github.com/user-attachments/assets/4985bed7-fd0b-4649-8f7b-272ad21a88af)

- Name functions and variables with lowercase characters, with words separated by underscores.

- Follow DRY (Don’t Repeat Yourself) principles, creating maintainable and reusable code.

- Use concise logic and creative engineering where possible.

<h3>5. Code Comments</h3>

- Be well commented with concise, relevant notes that other developers can understand.
