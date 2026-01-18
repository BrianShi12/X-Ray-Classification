In addition to training and evaluating a model, please also include a writeup via a .md file discussing your implementation choices, model performance, and the project’s further implications in society. Alongside the coding portion of the project, a detailed analysis in your writeup is equally important! Please include the following in your submission:

At the top, write your first and last name, as well as your USC email address.
In one or two sentences, present your project to us!
Dataset: Indicate the dataset you chose to use, any preprocessing steps that were applied, as well as the reasoning behind these choices.
Model Development and Training: Discuss your model implementation choices, the training procedure, the conditions you settled on (e.g., hyperparameters), and discuss why these are a good set for your task.
Model Evaluation/Results: Present the metrics you chose and your model evaluation results. 
Discussion: 
How well does your dataset, model architecture, training procedures, and chosen metrics fit the task at hand? 
Can your efforts be extended to wider implications, or contribute to social good? Are there any limitations in your methods that should be considered before doing so?
If you were to continue this project, what would be your next steps?



Brian Shi, brianshi@usc.edu 

This project is about classifying X-Ray images into three categories: normal, pneumonia, and tuberculosis. To preprocess the data, I used the torchvision library to load the data and apply transformations to the images like resizing, normalizing, color jittering, and horizontal flipping. I used a ResNet18 model as my base model and added a fully connected layer at the end to output the three classes. I used cross entropy loss and Adam optimizer to train the model. I used a learning rate of 2e-4 and trained the model for 20 epochs. Additionally, I noticed an imbalance in the dataset, and to offset that imbalance, I weighted the loss function to give more weight to the minority classes using an sklearn function. I used accuracy as my metric to evaluate the model. The final test accuracy was 77.73%. My model can be extended to wider implications by actually being implemented in a hospital setting and helping doctors and medical professionals to diagnose diseases more accurately and efficiently. Before doing so, many things should be taken into consideration, such as the quality of the data, the accuracy of the model, and the ethical implications of using AI in medical diagnosis. My next steps would be to do just that, and to continue to improve the model by using more advanced techniques and larger datasets.