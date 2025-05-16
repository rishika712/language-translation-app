# 🌍 Language Translator (English to French) using Sequence-to-Sequence Model

This project implements a **machine learning-based English-to-French language translator** using a **Sequence-to-Sequence (Seq2Seq)** model with encoder-decoder architecture. It demonstrates how deep learning can be used for natural language translation from one language to another.

## 🎯 Project Objective

- Translate English sentences into French using an LSTM-based sequence model.
- Train the model on a dataset of English-French sentence pairs.
- Provide a GUI to allow users to input English text and receive French translations.

## 📁 Project Structure

language-translator-ml-codes/
├── eng-french.txt # Dataset of English-French sentence pairs
├── langTraining.py # Model training script
├── training_data.pkl # Saved tokenized data and sequences
├── LangTransGui.py # GUI for translation using trained model
└── README.md # Project documentation

## 🛠️ Technologies Used

- **Language**: Python  
- **Libraries**:
  - NumPy
  - TensorFlow / Keras
  - Tkinter (for GUI)
  - Pickle (for storing preprocessed data)

## 🚀 How to Run the Project

### 1. Clone the Repository

git clone https://github.com/rishika712/language-translation-app.git
cd language-translation-app/language-translator-ml-codes

### 2. Install Dependencies

pip install numpy tensorflow

### 3. Train the Model (Optional)
If you want to retrain the model:

python langTraining.py
This will generate a trained model and save tokenized sequences as training_data.pkl.

### 4. Run the Translator GUI

python LangTransGui.py
This will launch a simple Tkinter GUI where you can input English sentences and get real-time French translations.

## 🧠 How It Works

Data Preparation: The dataset (eng-french.txt) contains English-French sentence pairs. Sentences are cleaned, tokenized, and padded.

## Model Architecture:

Encoder: LSTM that processes the input English sentence.

Decoder: LSTM that generates the French translation based on encoder states.

Training: Uses teacher forcing for efficient learning.

Inference: During prediction, the trained decoder predicts one word at a time until it reaches an end-of-sequence token.

## 📄 License

This project is licensed under the MIT License.


