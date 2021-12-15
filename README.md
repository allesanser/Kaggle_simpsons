# Kaggle_simpsons
This repository shows the work, submitted as part of the coursework from the Deep Learning School. The coursework was set as an in-class Kaggle competition. 


# Data
The data consisted of:

20933 labeled images, which were used for training and model validation
991 unlabeled images, for which class labels needed to be provided (test set)
The images were unevenly split across 42 different characters (classes).

# Metric
The metric used in a competition was the mean F1-Score, which is commonly used for multiclass classification problems such as this one.

# Goal
The coursework was marked according to performance on the Kaggle public test set. All works with F1-score above 0.97 were awarded full marks.

Achieving F1-score of more than 0.97 on the test set with less than 10 submissions became the primary goal of this project. The restriction on the number of submissions is useful not to overfit on the public score of the test set, since at this point it stops reflecting true generalisation performance (see more in a blog post by Moritz Hardt).

# Fine-tuning EfficientNet-b2 (3 + 30 epochs with early-stopping)
I needed a model with good computational complexity. The recently developed by Mingxing Tan and Quoc V. Le EfficientNet provided exacly a solution like that. Like ResNet, EfficientNet comes with different versions each of which requires different computational resources for the training to converge. I decided to use one of the lighter versions, of EfficientNet-b2 to keep the computational cost similar to one of ResNet-18.
Score on Kaggle: 0.99574
