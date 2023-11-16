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


In summary, underfitting is a situation where a model is too simplistic to represent the data, leading to poor performance. The goal is to strike a balance between model complexity and data representation to avoid underfitting and overfitting.