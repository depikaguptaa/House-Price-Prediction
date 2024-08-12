# House Price Prediction Web App

This project is a Flask-based web application that predicts house prices using a machine learning model. The app allows users to input various house features, such as BHK, square footage, number of bathrooms, furnished status, and location, and returns an estimated price based on the trained model.

## Features

- **User Input Form**: A web form that allows users to input house features.
- **Price Prediction**: The application returns an estimated house price based on user input.
- **Model Integration**: The app uses a pre-trained machine learning model to make predictions.
- **Responsive Design**: The application is designed to be responsive and can be accessed on both desktop and mobile devices.

## Environment Setup

To set up the environment for this project, follow these steps:

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/depikaguptaa/house-price-prediction.git
2. **Navigate to the Directory:**

    ```bash 
   cd house-price-prediction
3. **Create the Environment:**
    
    Run the following command to create a conda environment in the venv directory:

    ```bash
    conda create -p venv python -y
4. **Activate the Environment:**

    Activate the environment using:
    ```bash
    conda activate venv
5. **Install Dependencies:**

    Install Flask and other dependencies from ```requirements.txt``` using:
    ```bash
    pip install -r requirements.txt
## Running the Application

Once the environment is set up and all dependencies are installed, you can run the web application by executing:
```bash 
python app.py
```   
This will start the Flask development server. Open your web browser and navigate to ```http://localhost:5000``` to access the application.

## Project Structure

    house-price-prediction/
    │
    ├── app.py                # Main application file
    ├── venv/                 # Conda virtual environment directory
    ├── dataset/              # Dataset used for Model Training
    |   └── House_Rent_Dataset.csv
    ├── templates/            # HTML templates for the web application
    │   └── index.html        # Main page template
    ├── static/               # Static files (CSS, JS, images)
    │   └── styles.css        # CSS styling for the app
    ├── model/                # Directory for machine learning model files
    │   └── model.pkl         # Trained model in pickle format
    |   └── model.py          # Trained model python file
    ├── requirements.txt      # List of dependencies
    └── README.md             # This is README file

## How the Model Works

The machine learning model used in this project was trained using a dataset containing various features of houses and their corresponding prices. The model uses these features to learn patterns and predict prices for new data.

### Model Training:

The model was trained using the following steps:

1. **Data Preprocessing:** Cleaning and preparing the data for training.

2. **Feature Engineering:** Selecting relevant features that influence house prices.

3. **Model Selection:** Choosing a suitable machine learning algorithm (e.g., Linear Regression, Random Forest, etc.).

4. **Training:** Training the model on the dataset.

5. **Evaluation:** Evaluating the model's performance using metrics like RMSE (Root Mean Squared Error).

### Model Deployment:

The trained model is saved as a ```.pkl``` file and loaded into the Flask app for making predictions.


## Future Enhancements

1. **Model Improvement:** Explore and implement more advanced algorithms to improve prediction accuracy.

2. **Feature Expansion:** Add more features to the model, such as proximity to amenities, neighborhood ratings, etc.

3. **User Authentication:** Implement user login and profile management.

4. **Data Visualization:** Integrate graphs and charts to visualize price trends and distributions.
