# Formula 1 race winner prediction app

## Overview
This repository contains code for predicting the probability of a Formula 1 driver winning a race based on historical driver standings data.

## Requirements
- Python 3
- pandas
- scikit-learn
- TensorFlow

## Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/your_username/f1_race_predictor.git
   cd f1_race_predictor
   
2. Install the required packages:
   ```bash
   pip install -r requirements.txt

3. Prepare your dataset:

   - Ensure your dataset is in CSV format.
   - Update the path to your dataset in the code: df = pd.read_csv('driver_standings.csv')

4. Train the model:
   - Run the script to train the neural network model:
      ```bash
      python train_model.py

5. Evaluate the model:

   - The model will be evaluated automatically during training.
   - After training, the model accuracy will be displayed.

6. Make predictions:

   - Run the prediction script:
     ```bash
     python predict.py
  
   - Follow the prompts to enter race and driver information.
   - The predicted win probability for the specified driver in the specified race will be displayed.

## Model Details

- The model architecture consists of a neural network with two hidden layers.
- Binary classification is performed using the sigmoid activation function.
- The model is trained using binary cross-entropy loss and the Adam optimizer.

## File Structure

- 'driver_standings.csv': Sample dataset containing historical driver standings.
- 'train_model.py': Script for training the neural network model.
- 'predict.py': Script for making predictions using the trained model.
- 'f1_model.h5': Trained model saved in HDF5 format.
- 'requirements.txt': List of required Python packages.

## Input Data Format

- The input data should include the following features:
  - 'raceId': Race ID (integer)
  - 'driverId': Driver ID (integer)
  - 'points': Points scored by the driver (integer)
  - 'wins': Number of wins by the driver (integer)

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

Feel free to customize it further based on your preferences or additional details you want to include!
