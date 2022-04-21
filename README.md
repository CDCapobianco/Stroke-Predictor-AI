# Stroke-Predictor-AI
A small binary classification ML program which predicts stroke probability based on the medical status of the patient


# Description
The CSV dataset contains 10 features (+ label) and looks like this
<img width="836" alt="Immagine 2022-04-21 173817" src="https://user-images.githubusercontent.com/100691347/164498087-7aa99045-cb39-419a-b518-7a5f17a51655.png">

Before being fed to the ANN, the dataset is split,encoded and scaled in [0,1] range, using the Sci-Kit Learn library for Python.

The ANN architecture used is super simple and it's implemented with tf.Sequential

<img width="399" alt="Immagine 2022-04-21 174528" src="https://user-images.githubusercontent.com/100691347/164499740-762807df-d28c-46dd-bd7b-2437c21c50dd.png">


The model gets roughly 94 percent accuracy without any adjustment. It's worth saying that "shallow" ML models like SVM could also probably get a quite decent score for this kind of binary classification task.
Probably there's still room for improvement.
