Translation Model with Evaluation Metrics and Cross-Validation

Overview

This project utilizes the Helsinki-NLP MarianMT Model for English-to-French translation. It assesses translation quality using BLEU, METEOR, and TER scores while also performing hyperparameter tuning and cross-validation on a simulated dataset.

Dependencies

Ensure the following Python libraries are installed:
pip install torch transformers nltk sacrebleu scikit-learn numpy

Features

Machine Translation: Translates English text to French using Helsinki-NLP/opus-mt-en-fr.
Hyperparameter Tuning: Simulates tuning of learning rate and batch size.
Evaluation Metrics:
BLEU Score: Measures similarity to reference translations.
METEOR Score: Assesses semantic similarity.
Translation Edit Rate (TER): Evaluates edit distance.
Cross-Validation: Simulates model training using KFold.

Usage

Run the script with:
python translation_evaluation.py

Expected Output

Translated Text: ['Bonjour, comment ça va ?']  
Best Hyperparameters: Learning Rate=0.001, Batch Size=32, Score=0.92  
BLEU Score: 0.8  
METEOR Score: 0.75  
TER Score: 20.5  
Average Cross-Validation Accuracy: 0.85  

File Structure

project_folder/
│── main.ipynb   # Main script  
│── README.md                   # Documentation  

Notes

The dataset for cross-validation is simulated; replace it with real embeddings for practical use.
Hyperparameter tuning is currently randomized for demonstration purposes.

Future Improvements

Fine-tuning the MarianMT model on a custom dataset.
Implementing a more advanced hyperparameter tuning method (e.g., Optuna).
Using real-world data for cross-validation.

License

This project is open-source under the MIT License.
