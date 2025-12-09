Tags: #Perceptron #NeuralNetwork 

**Perceptron**:
- Simplest form of a neural network
- Consists of a single neuron with adjustable synaptic weights and bias.
- It performs pattern classification with only two classes
- Perceptron convergence theorem:
  1. Patterns (vectors) are drawn from two linearly separable classes
  2. During training, the perceptron algorithm converges and positions the decision surface in the form of hyperplane  between two classes by adjusting synaptic weights.

**Characteristics of a Perceptron**:
- a machine learning algorithm for the supervised learning of binary classifiers
- The weight coefficient is automatically learned.
- Initially, weights, and input features are multiplied. Next, the decision is made whether the neuron should be not fired or fired. 
- The **activation function** in any perceptron learning algorithm example employs a step rule to determine whether the weight function's value is higher than zero.
- If the sum of all input values is higher than the threshold value (**Bias**), it should have an output signal; else, no output is displayed.
- The linear decision boundary is plotted and it enables the distinction between the two linearly separable classes "+1" and "-1".

**Discrete Perceptron**: Gives a hard, final verdict (Yes or No). (Yes or No)
**Continuous Perceptron**: Gives a nuanced "confidence score" or probability (How much?). (There is a 12% chance it is No)

**Application:** Perceptron is used for classification. 

*Example:*
	- If the output of the perceptron is +1 then the input is assigned to the class C1
	- If the output of the perceptron is -1 then the input is assigned to class C2.

**Classification**: 

*If the perceptron gives a wrong undesirable output, then one of two things could have happened.*
- The desired output is 0, but the net input is above threshold. So the actual output becomes 1. In such a case we should decrease the weights.
- The desired output is 1. but the input is below threshold. We should now increase the weights.

**Limitations**: The perceptron can only model linearly separable functions.
*Linearly Inseparable*: arranges data in a way that is impossible to separate with a single straight line. 
- XOR is **not linearly separable**

**Different Non-Linearly Separable Problems**
1. Half Plane Bounded By Hyperplane
2. Convex Open or Closed Regions
3. Arbitrary (Complexity Limited by No. of Nodes)

**Perceptron Algorithm**:
1. Set a threshold value
2. Multiply all inputs with its weights
3. Sum all the results
4. Activate the output

**Bias: the target number is always 0**
**Threshold: target number changes**