# SHL_ASSESSMENT

This project shows how I integrated speech recognition, NLP-based feature engineering, and a deep learning regression model to build an end-to-end grammar scoring system.

>I used OpenAI's Whisper model to transcribe audio files into text.

>Then, I extracted language features from the transcriptions using spaCy (for sentence structure) and LanguageTool (for grammar error detection).

>I also included a readability metric using textstat (Flesch reading ease score).

>These extracted features were used to train a regression model using TensorFlow and Keras to predict a grammar quality score for each transcript.

#about the files saved:

>The extracted features from all training samples are saved in a CSV file named feature_file.csv, which allows easy reuse without reprocessing the audio files.

>The trained model is saved as model, which can be reloaded and used directly for prediction.

#Testing:

>After training, the model was used to predict grammar scores on the audio data provided in kaggle, and scores were generated based on transcriptions and extracted features.

>The predictions are saved in a file called grammar_score_predictions.csv, which contains the predicted grammar quality scores for each test audio file.
