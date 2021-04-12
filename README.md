# CGM_GSOC
Evaluation Test

- notebook.ipynb - contains full code
- scaler - pickle file, SkLearn Robust Scaler
- saved_encoder - Tensorflow saved model, encoder used to transform features to low dimensional space 
- clf_red - pickle file, XGBoost classification model, accept low dimensional features as input
- clf - pickle file, XGBoost classification model, accept original features as input
- saved_model - Tensorflow saved model, Autoencoder, used to train encoder 

Load pickle file using python `pickle` module

Load TensorFlow model using, `tensorflow.keras.models.load_model` function
