# DecisionTree
Three types of decision trees
1 implement a decision tree learning algorithm
2 run experimentson real datasets

Data sets :
BALLOONS: These are four very small files you can use to test your program on. They are simple enough that you will know the correct answer (see balloon.info) and each feature is binary and there are only two classes. There are no test or pruning sets provided, this data is provided for you to test your basic learning algorithm.

HYPOTHYROID: This is a medical database representing the classification of 3163 patients with and without hypothyroid disease at the Garavan Institute of Sydney, Australia.

MESSIDOR: This dataset contains features extracted from the Messidor image set to predict whether an image contains signs of diabetic retinopathy or not. All features represent either a detected lesion, a descriptive feature of a anatomical part or an imagelevel descriptor.

Implementation:

1. For each of the data sets was the decision tree algorithm able to memorize the training data (i.e., get 100% accuracy when used to classify the training data)? If not, can you give at least one reason that you think it was not able to?
2. Could you use your system to, say, buy stocks or bet on horses? Why or why not? 

Balloon:
1. Demonstrate your program on these small data sets. Draw out the trees you generated for the 4 balloon examples. Note that there are no testing or pruning files—we assume your tree will be perfect in these very simple examples.

Hypothyroid and Messidor:
1. What is the majority class accuracy for the test set? (i.e. what is the accuracy to just say "benign" always?)
2. How does you tree’s test accuracy compare to the majority accuracy?
3. What do the top 2 levels (the root and the level just below) look like (draw them)?

Use reduced-error pruning. This is a pruning criterion that replaces a subtree with a single leaf when that leaf (which classifies the instance as the majority class of all instances seen at that leaf during pruning) represents a lower error rate than does the subtree. The pruning procedure thus has the following steps:
Grow the tree fully on the training data.
In a postorder recursive fashion traverse the decision tree, replacing a non-leaf node with a leaf node only when the error rate of the subtree node exceeds the error rate of the leaf node. Measure the error rate on a separate set of instances (called the pruning data).

Explore the effect of Bagging. Choose the data set for which you performed the WORST, and see if you can improve your results via bagging.

Explore the effect of Boosting. Choose the data set for which you performed the WORST, and see if you can improve your results via implementing the AdaBoost ensemble algorithm.
