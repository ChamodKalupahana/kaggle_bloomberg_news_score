# PSL Week Prediction using Bloomberg News

This repository contains a Python notebook that explores and predicts PSL (Pakistan Super League) week sentiments using Bloomberg News data. The notebook utilizes TensorFlow and LSTM (Long Short-Term Memory) networks for the prediction task.

## Dataset
The dataset is loaded from the following CSV files:
- `/kaggle/input/2023-psl-week-using-bloomberg-news/train.csv`
- `/kaggle/input/2023-psl-week-using-bloomberg-news/test.csv`

The training dataset has the following columns:
- `Unnamed: 0`: Date
- `positive`: Number of positive sentiments
- `negative`: Number of negative sentiments
- `indecisive`: Number of indecisive sentiments
- `score`: Sentiment score
- `y`: Target variable

## Exploratory Data Analysis (EDA)

The notebook begins with an exploration of the dataset, including a summary of statistical measures and visualizations of sentiment trends over time.

## Data Preprocessing

The dataset is preprocessed to prepare it for the model. This includes normalizing sentiment counts and creating input and output arrays (`x` and `y`).

## Model Architecture

The LSTM model is defined with the following layers:
- Input Layer (1D data)
- LSTM layers with different units
- Dense layers with various units and activation functions

The model is compiled using Mean Absolute Error as the loss function and the Adam optimizer.

## Training

The model is trained on the training dataset for 50 epochs with a batch size of 32.

## Model Evaluation

The trained model is evaluated on the test dataset, and predictions are generated for PSL week sentiments.

## Submission

The predictions are saved in a CSV file (`submission.csv`) in the `/kaggle/working/` directory.

Feel free to explore the notebook for a detailed walkthrough of the analysis and modeling process.
