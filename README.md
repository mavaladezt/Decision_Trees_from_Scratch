### Decision Trees - Regression (numpy)

#### Decision Trees
Decision Trees are predictive classifiction algorithms which split (branch) training data in a way that they can reach a conclusion (leaf). The tree is then used to predict the values using the test dataset.<br>
There are different 'ways' this trees 'decide' where and in what order to split (here are a couple of them):<br>
 - Gini impurity: very usefull when dataset has labels
 - Variance reduction: used when labels take the form of continuous numbers

Decision trees where the target variable can take continuous values (typically real numbers) are called regression trees.<br>

#### Regression Trees
Decision trees where the prediction label are real numbers.<br>

__In the following implementation we will be using only numpy.__

The data was obtained from:<br>
__Dua, D. and Graff, C. (2019). UCI Machine Learning Repository (https://archive.ics.uci.edu/ml/datasets/Car+Evaluation). Irvine, CA: University of California, School of Information and Computer Science.__<br>

Abstract: The model evaluates cars according to the following concept structure:<br>


__Class Values__: unacc, acc, good, vgood 

__Attributes:__<br>
__buying__: vhigh, high, med, low.<br>
__maint__: vhigh, high, med, low<br>
__doors__: 2, 3, 4, 5more<br>
__persons__: 2, 4, more<br>
__lug_boot__: small, med, big<br>
__safety__: low, med, high<br>

(we will be transforming the dataset so we can have numbers instead of strings)