# Dimensionality Reduction Using AutoEncoder
See: [notebook.ipynb](https://github.com/utkarsh-21st/dimensionality-reduction-using-auto-encoder/blob/main/notebook.ipynb "notebook.ipynb")
- Used XGBosst for classification and keras for building an AutoEncoder

- Link to the dataset: https://drive.google.com/file/d/1Nl-RU5HggCSWWqINN4gbxHAVzER6T2Po/view?usp=sharing
##### Result on test data:
- with original features (dimensions=28), ROC AUC Score = 0.8430741138771947
- with low dimensional features (dimensions=14), ROC AUC Score = 0.736416256396276
- Pipeline:
original features -> Robust scaler -> low dimensional features -> DMatrix -> XGBoost
-----
##### Info
- notebook.ipynb - contains full code
- scaler - pickle file, SkLearn Robust Scaler
- saved_encoder - Tensorflow saved model, encoder used to transform features to low dimensional space 
- clf_red - pickle file, XGBoost classification model, accept low dimensional features as input
- clf - pickle file, XGBoost classification model, accept original features as input
- saved_model - Tensorflow saved model, Autoencoder, used to train encoder 

Load pickle file using python `pickle` module

Load TensorFlow model using, `tensorflow.keras.models.load_model` function
