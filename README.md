# XAI_Research-Explainable-Neural-Networks
This research aims to analyze the main techniques of XAI (Explainable Artificial Intelligence), primarily applied to neural networks. The analyzed techniques are as follows:<br><br>
**##NAM (Neural Additive Models) described in the paper "Neural Additive Models: Interpretable Machine Learning with Neural Nets" by Rishabh Agarwal et al., 2020.** It has been applied to the Heart Disease Dataset for binary classification. Here, you'll find the implementation from scratch of a NAM neural network using NumPy, SciPy, and JAX for automatic differentiation (AutoGrad). The result is a neural network where each feature is analyzed independently, providing the opportunity to interpret the results of a model considered as a black-box.
<br><br>
<b>SHAP (SHapley Additive exPlanations) is a game theory approach to explain the output of any machine learning model. </b> In this case, it's applied to the California Housing Dataset for regression and is able to distinguish which parts of the data are important and which are not. Finally, various graphs are shown explaining the contribution of each feature, both positive and negative, and how they interact with each other towards the final prediction. This is one of the most general tecniques and it can be similarly utilized for other types of problems as well.
<br><br>
**Adversarial Attack applied to the MNIST dataset for multiclass digit classification.** Here, we exploit the ability to differentiate the neural network with respect to its inputs rather than with respect to its weights and biases in order to induce errors. By varying a reference image towards the direction of the gradient, we can obtain very similar images with different labels and completely different images with the same label. Furthermore, we can also generate an image that represents the most likely outcome for a certain label, and we observe that it is completely different from what we would expect. These findings suggest that the neural network is not easily explainable, and it would be better to try a convolutional network to overcome this issue.
<br><br>
**EBM (Explainable Boosting Machines).** In this notebook, you'll see how to implement a decision tree from scratch for both binary and multiclass classification problems. This is the typical machine learning model used when it's important to understand the reasoning of the algorithm, as it allows drawing the tree and its various branches where each feature is analyzed. Entropy measurement is done using the Gini coefficient. The final decision tree, modeled as a nested hash map, can be used both for prediction and for analyzing the weight of each feature. This approach can be enhanced with Bagging and Boositng, giving life to the famous Random Forest Algotithm.
