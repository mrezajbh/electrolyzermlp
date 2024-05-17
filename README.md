# electrolyzermlp
Electrolyzer MPL
Electrolyzer Performance Prediction with MLP Model
This code implements a machine learning model to predict the performance of a proton exchange membrane (PEM) electrolyzer. The model is trained on a simulated dataset containing 5,000 data points, each representing a unique combination of input parameters and the resulting output performance metrics.

Key Features
Multilayer Perceptron (MLP): The model architecture is a Multilayer Perceptron neural network, which is suitable for learning complex relationships between input variables and output performance metrics.
Hyperparameter Tuning: Randomized search is used to explore different model configurations, identifying the best combination of hyperparameters (number of layers, neurons per layer, dropout rate, batch size) to maximize model performance.
Performance Evaluation: The model's performance is rigorously evaluated using multiple metrics (mean squared error, R-squared) and visualized with scatter plots and bar charts for each output variable.
Interpretability: Learning curves are plotted to assess the model's training progress and identify potential overfitting issues.
How to Use the Code
Prerequisites:

Python 3.x
Required libraries (install using pip install pandas numpy scikit-learn scikeras tensorflow matplotlib)
Dataset: full result clean.csv (available in the repository)
Running the Code:

Execute the script.
The script will:
Load the dataset
Preprocess the data (standardization, train-test split)
Perform hyperparameter tuning using randomized search
Train the best model on the training data
Evaluate the model on the test data
Display performance metrics and visualizations
Interpreting the Results:

Examine the bar charts for MSE and R-squared values to assess the overall performance of the model.
Look at the scatter plots (actual vs. predicted) to understand how well the model predicts each output variable individually.
Analyze the learning curves to ensure the model is not overfitting the training data.
Additional Notes
The dataset used for training and testing (full result clean.csv) was generated using Aspen Plus simulation software (version 14).
The model's performance is acceptable for most output variables, but there's room for improvement, especially for predicting H2OCIN. Feel free to experiment with different model architectures or hyperparameter configurations to achieve better results.
The code is open-source and available under the [Creative Commons Zero v1.0 Universal license (CC0 1.0)]([Link to the CC0 1.0 license]). Feel free to modify and use it for your research or educational purposes.
Contributing
If you find any issues or have suggestions for improvement, please open an issue or pull request in the GitHub repository.

Let me know if you'd like any other adjustments to this file.
