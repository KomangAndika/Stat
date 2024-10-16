## Underfitting
Underfitting is a term used in the context of machine learning and statistical modeling to describe a situation where a model is too simplistic to capture the underlying patterns in the data. When a model underfits the data, it means that the model's complexity is insufficient to represent the true relationship between the input features and the target variable. As a result, the model performs poorly, both on the training data and on unseen data (validation or test data).
![under vs over](https://github.com/KomangAndika/Stat/assets/108614290/db7ec436-99e1-45d3-808a-88fca7d3fd8a)

Key characteristics of underfitting include:

1. **High Bias**: Underfit models have high bias, meaning that they make overly simplified assumptions about the data. These assumptions can lead to a significant error, as the model cannot adequately represent the complexity of the underlying problem.
 
2. **Low Variance**: While high bias is a defining characteristic, underfit models typically have low variance. This is because they are so simple and constrained that they don't respond to fluctuations or noise in the training data.

3. **Poor Performance**: Underfit models perform poorly on the training data because they fail to capture the data's essential patterns. Additionally, they also perform poorly on unseen data (validation or test data) because they cannot generalize effectively.

4. **Linear Models Example**: One common example of underfitting is when you try to fit a linear model to data that has a more complex, non-linear relationship. In such cases, the linear model may not capture the curvature or intricacies of the data and, as a result, underfit.


To address underfitting, you can consider the following strategies:

- Increase Model Complexity: Use a more complex model or algorithm that can capture the underlying patterns in the data. For example, if you are using a linear model and it underfits, you might try using a non-linear model.

- Feature Engineering: Carefully select and engineer relevant features that can help the model better represent the problem.

- Collect More Data: Sometimes, underfitting can occur when there is not enough data for the model to learn from. Collecting more data may help in such cases.

- Regularization: If you are using a complex model, you can use regularization techniques to prevent overfitting while still allowing the model to capture more complex patterns.


## OverFitting
Overfitting is a common problem in machine learning and statistical modeling. It occurs when a model is too complex or flexible and starts to fit the training data too closely, capturing noise and random fluctuations in the data. As a result, an overfit model performs very well on the training data but poorly on unseen or new data. Overfitting is a significant concern because it hinders a model's ability to generalize and make accurate predictions on real-world data.

Key characteristics of overfitting include:

1. **Low Bias**: Overfit models have low bias, meaning they are highly flexible and can fit the training data very closely. They often exhibit a good fit to the training data.
    
2. **High Variance**: High variance is a defining characteristic of overfitting. These models are so flexible that they capture noise and random variations in the training data.
    
3. **Excellent Training Performance**: Overfit models tend to perform exceptionally well on the training data, often achieving near-perfect accuracy.
    
4. **Poor Generalization**: The problem with overfitting is that the model's performance degrades significantly when applied to new, unseen data. It doesn't generalize well, as it has essentially memorized the training data rather than learned the underlying patterns.
    

To address overfitting, you can consider the following strategies:

1. **Simplify the Model**: Reduce the complexity of the model by using a simpler algorithm or by reducing the number of features or parameters. For example, in the case of decision trees or ensemble methods like Random Forests, you can limit the depth of the tree to reduce complexity.
    
2. **Regularization**: Use regularization techniques (e.g., L1 or L2 regularization) to penalize large coefficients or complex model structures, which can help prevent overfitting.
    
3. **Cross-Validation**: Employ cross-validation to assess your model's performance on multiple subsets of the data. This helps you understand how well your model generalizes and whether it's overfitting.
    
4. **More Data**: Collecting more data can sometimes help mitigate overfitting, as it provides the model with more information to learn from. However, this may not always be feasible.
    
5. **Feature Selection**: Carefully choose and engineer relevant features while excluding irrelevant or noisy features.
    
6. **Early Stopping**: When training iterative models (e.g., neural networks), use early stopping techniques to halt training once the model's performance on a validation dataset starts to degrade.
    

Balancing the trade-off between bias and variance is a fundamental challenge in machine learning. The goal is to find a model that is complex enough to capture the underlying patterns in the data but not so complex that it overfits the training data, thus achieving good generalization performance.

In summary, underfitting is a situation where a model is too simplistic to represent the data, leading to poor performance. The goal is to strike a balance between model complexity and data representation to avoid underfitting and overfitting.