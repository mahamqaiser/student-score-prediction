# Student Score Prediction

This project predicts students' exam scores based on various features using Linear Regression. It includes steps for data loading, preprocessing, model training, evaluation, and visualization. The dataset (`student_score.csv`) should contain both numerical and/or categorical features (e.g., study hours, attendance, difficulty level) and a target column for scores (default: "Exam_Score" — change this in the script if your dataset uses a different name). 

## Requirements
- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

Install dependencies with:
pip install pandas numpy matplotlib seaborn scikit-learn

## How It Works
1. **Data Loading**: Reads the dataset from the provided CSV file path.
2. **Data Cleaning**: Handles missing values using forward fill.
3. **Encoding**: Converts categorical columns into numeric form using Label Encoding.
4. **Data Splitting**: Splits the dataset into training (80%) and testing (20%) sets.
5. **Model Training**: Uses scikit-learn’s LinearRegression to train the model.
6. **Prediction**: Predicts scores for the test dataset.
7. **Evaluation**: Measures performance using Mean Absolute Error (MAE), Mean Squared Error (MSE), and R² Score.
8. **Visualization**: Creates a scatter plot for Actual vs Predicted scores and a histogram for prediction error distribution.

## Running the Project
1. Place your dataset file (`student_score.csv`) in the path specified in the script or update the file path in:
   df = pd.read_csv(r'C:\Users\LENOVO\Documents\student_score.csv')
2. Run the script:
   python student_score.py

## Example Output
Model Performance:
Mean Absolute Error: 4.23  
Mean Squared Error: 25.47  
R² Score: 0.89  

Two plots will be displayed:
- Actual vs Predicted Scores
- Error Distribution

## Notes
- If your dataset's score column name is different from "Exam_Score", update the variable `target_column` in the script.
- You can experiment with other algorithms (e.g., RandomForestRegressor, GradientBoostingRegressor) for better results.

## License
This project is open-source and available for educational purposes.
