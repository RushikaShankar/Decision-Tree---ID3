# Decision Tree-ID3
## Decision Tree using ID3 Algorithm 

### Decision Tree
A decision tree mimics human decision-making. It represents decisions and their possible consequences in a tree-like structure:

- Root Node: The topmost decision 

- Internal Nodes: Tests on features 

- Branches: Outcomes of those tests 

- Leaf Nodes: Final decisions or predictions 

#### ✅ Pros
- Easy to understand and visualize
- Requires little data preprocessing
- Handles both numerical and categorical data

#### ❌ Cons
- Prone to overfitting
- Unstable (small changes in data can change the tree)
- Greedy algorithm — may not find the optimal tree



###  What is ID3?

ID3 is a classic algorithm introduced by **Ross Quinlan**. It constructs a decision tree by recursively selecting the feature that yields the highest information gain. The resulting tree can be used to classify new instances by traversing the tree based on their feature values.

#### How ID3 Works – Step by Step
1. Calculate Entropy of the current dataset.

2. For each feature:
   - Calculate the Information Gain of splitting on that feature.
   - Choose the feature with the highest Information Gain as the decision node.

3. Split the dataset based on this feature.

4. Repeat steps 1–4 recursively for each subset of data, until:
   - All instances in a subset belong to the same class, or
   - There are no more features to split on.
  
#### ✅ Advantages
- Simple and easy to implement
- Works well with categorical features
- No need for parameter tuning

#### ❌ Limitations
- Only works with categorical data (extensions like C4.5 handle numerical)
- Can overfit if not pruned
- Greedy: makes locally optimal decisions which may not be globally optimal

 

## 🧠 Core Concepts

- **Entropy**: Measures the impurity or randomness in the dataset.
- **Information Gain**: Reduction in entropy after splitting on a feature.
- **Recursive Tree Building**: Splitting continues until all samples in a node belong to the same class or no more features remain.

##  Implementation

This implementation includes:

- Dataset preprocessing
- Entropy and information gain calculations
- Recursive tree construction
- Prediction using the learned tree
- (Optional) Visualization of the decision tree structure

## Acknowlwgement 
https://github.com/Victor-Ikechukwu Thank you for your invaluable insights, feedback, and continuous support throughout the development of this project.
