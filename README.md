# California House Price Prediction

This project implements a machine learning model to predict house prices in California based on various features such as median income, house age, average rooms, population, and location coordinates. The model is deployed as a web application where users can input house features and get price predictions in real-time.

## Features

- Machine Learning model built using Scikit-learn
- Interactive web interface for real-time predictions
- Data visualization and analysis using Seaborn and Matplotlib
- RESTful API endpoint for predictions
- Responsive UI design
- Model persistence using pickle

## Dataset

The project uses the California Housing dataset which contains information about houses in California. Features include:
- Median Income
- House Age
- Average Rooms
- Average Bedrooms
- Population
- Average Occupancy
- Latitude
- Longitude

## Tech Stack

- **Python 3.7**
- **Web Framework**: Flask
- **ML Library**: Scikit-learn
- **Data Processing**: Pandas, NumPy
- **Data Visualization**: Matplotlib, Seaborn
- **Frontend**: HTML, CSS
- **Model Serialization**: Pickle

## Setup Instructions

1. Clone the repository
```bash
git clone https://github.com/pauldebanshu19/californiahousepricing.git
cd californiahousepricing
```

2. Create a conda environment
```bash
conda create -p venv python==3.7 -y
conda activate venv/
```

3. Install required packages
```bash
pip install -r requirements.txt
```

4. Install the IPython kernel for Jupyter
```bash
conda install -p venv ipykernel --update-deps --force-reinstall
```

## Usage

1. Start the Flask application
```bash
python app.py
```

2. Open your web browser and navigate to `http://localhost:5000`

3. Enter the required house features in the form:
   - Median Income of the area
   - House Age
   - Average number of Rooms
   - Average number of Bedrooms
   - Population of the area
   - Average Occupancy
   - Latitude
   - Longitude

4. Click "Predict" to get the estimated house price

## Model Training

The model training process can be found in the `Linear Regression.ipynb` notebook, which includes:
- Data preprocessing
- Exploratory Data Analysis
- Feature Engineering
- Model Selection
- Model Evaluation
- Model Persistence

## Project Structure

```
californiahousepricing/
├── Linear Regression.ipynb    # Model training notebook
├── app.py                    # Flask application
├── regmodel.pkl             # Serialized model
├── templates/               # HTML templates
│   └── home.html           # Main prediction page
├── requirements.txt        # Project dependencies
└── README.md              # Project documentation
```

## Model Performance

The model achieves the following metrics on the test set:
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R-squared Score

## Future Improvements

- Add feature importance analysis
- Implement more advanced ML models
- Add cross-validation
- Include more visualization options
- Add model retraining capability
- Implement error handling and input validation

## Contributing

Feel free to fork this repository and submit pull requests to contribute to this project. You can also open issues for any bugs found or feature suggestions.

## License

This project is open source and available under the [MIT License](LICENSE).