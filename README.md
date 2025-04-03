# Iris_Flower Classifier

This project will classify iris flowers based on the given inputs into their respective species. The algorithm is implemented using a Sequential neural network with categorical cross-entropy as the accuracy metric.

The problem is comprised of 150 observations of iris flowers from three different species.

Classification is done on features:
1. sepal length
2. sepal width
3. petal length
4. petal width (all in the same unit of centimeters).

The predicted attribute is the species, which is one of Iris-setosa, Iris-versicolor, or Iris-virginica.

## Installation

To set up the project, clone the repository and install the required packages:

```bash
git clone https://github.com/akshargrover/Iris_Flower_Classifier.git
cd Iris_Flower_Classifier
pip install -r requirements.txt
```

## Usage

To run the classification model, execute the following command:

```bash
python classify.py
```

You can also use the provided Jupyter Notebook for an interactive experience:

```bash
jupyter notebook iris_classifier.ipynb
```

## Model Architecture

The model is built using a Sequential neural network with the following layers:
- Input layer: Accepts the four features of the iris flowers.
- Hidden layers: Two dense layers with ReLU activation functions.
- Output layer: A softmax layer that outputs the probabilities of each species.

### Optimizer and Loss Function

The model utilizes the **Adam optimizer**, which is an adaptive learning rate optimization algorithm. It combines the advantages of two other extensions of stochastic gradient descent, namely AdaGrad and RMSProp. Adam is particularly effective for training deep learning models as it adjusts the learning rate for each parameter individually, leading to faster convergence.

The loss function used is **categorical cross-entropy**, which measures the dissimilarity between the predicted probability distribution and the true distribution. This loss function is suitable for multi-class classification problems, as it penalizes the model more when it is confident about an incorrect prediction.

## Results

The model achieves an accuracy of approximately 97% on the test dataset. You can visualize the results using the provided plots in the Jupyter Notebook.

## Contributing

Feel free to submit issues or pull requests if you have suggestions for improvements or new features.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
