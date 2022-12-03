```ad-tldr
- Neurons are just balls that hold a number from 0 to 1
  - A REALLY complex function that has a range of [0,1]
 
```
# Neurons
- Hold a value between 0 and 1
- Can be assigned weights (+ve or -ve)
- Compute weighted sum to be put as value for next layer (different each time)
- Sometimes we want a bias before we even consider chucking it into the sigmoid (more 0s when results aren’t significant enough)
- Weighted sums may yield ANY value but you know that neurons only take 0 to 1
	- Plugging the values into the sigmoid function fixes that :D

```ad-warning
Sigmoid Function is pretty old school and not used in modern Neural Networks anymore the Rectified linear unit proved to be easier to train (ReLU(α))
### ReLU(α) = max(0,α)
```

- This happens to ALL neurons in each layer
- Each neuron has its own weight 
- Experimenting with weights and biases yourself helps you get better insights on how to structure and layer your Neural Network moving forward
- Better to think that each Neuron is a function with range [0,1]

```ad-note
Learning is referring to getting the computer to find a valid setting for all the weights and biases to solve the problem at hand
```

# Layers
- Number of layers and structure of layers has lots of room for experiments
- Activation of one layer affects the activation of next layer
- Like human brain, some neurons firing cause other neurons to fire too!
- Brightest neuron in output layer → What network thinks “solution” is
- In a perfect world the second to last layer’s neurons corresponds to sub components of a problem
- Layers can help with dividing the problem into smaller problems

```ad-example
  1. Edges in a picture 
  2. Syllables in speech
```

# Notation
- Writing function of weighted sum can be quite confusing
- Represent with [[Linear Algebra|Matrix]] multiplication 
  - Represents weights,activation and biases in forms of vectors in a vector multiplication
  
```ad-hint
title: Rule
## $a^{\prime} = σ(Wa + b)$

a -> activation vector

W -> weight vector

i -> index 

b -> bias vector
```
