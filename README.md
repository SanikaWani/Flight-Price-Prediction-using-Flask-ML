# Flight Price Prediction Web Application

This project is a Flight Price Prediction web application built using Flask for both frontend and backend. The machine learning model used for prediction was trained on a dataset (`train.csv`) using algorithms including Linear Regression, SVM, XGBoost, and RandomForest. Among these algorithms, RandomForest demonstrated the best performance, achieving an accuracy of 73%.

## Project Structure

- `app.py`: Flask application containing routes for handling user requests and displaying predictions.
- `train.csv`: Dataset used for training the machine learning model.
- `model.joblib`: Pickle file containing the trained RandomForest model.
- `templates/`: Directory containing HTML templates for rendering the web interface.
- `static/`: Directory containing static files such as CSS stylesheets and client-side JavaScript files.

## Requirements

Ensure you have Python 3 installed, along with the following libraries:
- Flask
- pandas
- scikit-learn
- numpy

You can install the required libraries using pip:

```
pip install Flask pandas scikit-learn numpy
```

## Getting Started

1. Clone this repository:

   ```
   git clone <repository_url>
   ```

2. Navigate into the project directory:

   ```
   cd flight-price-prediction
   ```

3. Run the Flask application:

   ```
   python app.py
   ```

4. Open your web browser and go to `http://localhost:5000` to view the application.

## How it Works

1. **Training the Model**: The machine learning model was trained using the `train.csv` dataset, employing algorithms such as Linear Regression, SVM, XGBoost, and RandomForest.

2. **Web Application**: Flask is used to create a web application that takes user inputs (such as flight details) and displays the predicted price using the trained RandomForest model (`model.pkl`).

3. **Prediction**: When a user submits a form with flight details, the Flask backend processes this input, applies preprocessing (if necessary), and uses the trained model to predict the flight price. The predicted price is then displayed to the user.

## Notes

- The accuracy of the RandomForest model on the test dataset (`train.csv`) was measured at 73%, making it the chosen model for this prediction task.
- This application is designed for demonstration purposes and may require further enhancements for production use, such as additional error handling and input validation.


Feel free to contribute by forking the repository and submitting pull requests!
