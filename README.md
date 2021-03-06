# Automated Essay Scoring

    A Deep Learning model that predicts the score of a given input essay.

The dataset is from Kaggle ASAP competition which was provided by The Hewlett Foundation.

The mysite folder contains the Django app if you want an interactive demo.
Performance

The accuracy is calculated by Quadratic Weighted Kappa(QWK), which measures the agreement between two raters. The model architecture consists of 2 Long Short Term Memory(LSTM) layers with a Dense output layer. The final layer uses the Relu activation function. The QWK is calculated by training model on the dataset using 5-Fold Cross Validation and taking the average for all five folds.





# Requirements

    Tensorflow 1.9
    Keras 2.2.2
    Django 2.1
    Gensim 3.5

pip install tensorflow
pip install keras
pip install django
pip install gensim

Installation

    Clone the repo
    Just run the Jupyter Notebook to train the model.
    To run the Django App cd ./ into the mysite folder and run

python manage.py migrate
python manage.py runserver

References

    A Neural Approach to Automated Essay Scoring
    Automatic Text Scoring Using Neural Networks
