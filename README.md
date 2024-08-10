In this project, we embarked on a journey to predict car acceptability using decision trees, a popular machine learning technique. Our starting point was the car dataset from OpenML, which provided various features like 'buying', 'maint', 'doors', 'persons', 'lug_boot', 'safety', and a target class 'BinaryClass' to guide our predictions.

Before diving into model building, we took a closer look at the data. We split it into training and test sets, ensuring that we had a solid foundation to work from. Our first task was to check for any missing values and get a feel for the categorical features that dominated the dataset. This step was crucial in preparing the data for the next stages.

With the data cleaned and prepped, we moved on to the heart of the task: building a Decision Tree Classifier. Initially, the model seemed to perform well, but it soon became apparent that it was overfitting – a common issue where the model learns the training data too well and struggles to generalize to new, unseen data.

To overcome this, we decided to refine our approach. We reduced the maximum depth of the tree to prevent it from becoming too complex, and we addressed the imbalance in our dataset by adjusting the class weights. To fine-tune the model further, we employed GridSearch, which helped us find the best combination of hyperparameters.

Finally, with an improved model in hand, we tested it on our reserved test set. The results were encouraging: our model achieved an accuracy of 86%, with impressive precision, recall, and f1-scores. This journey taught us the importance of careful data preparation and thoughtful model refinement, leading to a robust solution that could generalize well beyond the training data.
