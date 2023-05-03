Download Link: https://assignmentchef.com/product/solved-cs-534-artificial-intelligence-assignment-3
<br>
<h1>Problem 1</h1>




<ol>

 <li>Implement your own k-means algorithm from the lecture slides using Python. (<strong>10 points</strong>)</li>

</ol>







<ol>

 <li>Using the k-means algorithm, cluster the data from the attached file <strong>txt</strong>. Plot X, Y coordinates for the entire dataset. Use different symbols and colors to represent your data points for different clusters.</li>

</ol>

Label X and Y axis as ‘Length’ and ‘Width’, correspondingly. Label each cluster as “Cluster 1”, “Cluster 2”, etc. <u>Explain your findings</u>. (<strong>5 points</strong>)







<h1>Problem 2</h1>




<ol>

 <li>Implement your own logistic regression with regularization algorithm from the lecture slides using Python. (<strong>10 points</strong>)</li>

</ol>







<ol>

 <li>Using the implemented algorithm, train and test the data from the attached file <strong>zip</strong>.</li>

</ol>

(<strong>10 points</strong>)

<ul>

 <li>Use 80% of each class data to train your classifier and the remaining 20% to test it.</li>

 <li>Run different values of logistic regression regularization parameter (λ). The range of λ is from -2 to 4 and the step is 0.2</li>

 <li>Plot the f-measure of the algorithm’s performance on the <strong>training and test sets</strong> as a</li>

</ul>

function of λ:




<em>f -measure</em>= 2<em>Pre</em><em>Rec Pre</em>+ <em>Rec</em>

<h2>                                                                   TP                      TP</h2>

where <em>Pre</em>= ;        <em>Rec</em>=    ; <em>TP </em>+ <em>FP        TP </em>+ <em>FN</em>




and <em>TP</em> is the number of true positives (class 1 members predicted as class 1),  <em>TN</em> is the number of true negatives (class 2 members predicted as class 2),  <em>FP</em> is the number of false positives (class 2 members predicted as class 1),  and <em>FN</em> is the number of false negatives (class 1 members predicted as class 2).




<ol>

 <li>Repeat the procedure in (b) but now using the features normalized with the <u>standardization</u> protocol discussed in the class. (<strong>5 points</strong>)</li>

</ol>
















<strong><u>In the following part of the assignment, you will be working on applying methods and</u></strong><strong> <u>datasets from the scikit-learn library</u>. </strong><strong> </strong>







<h1>Problem 3</h1>




Apply three clustering techniques to the handwritten digits dataset. Assume that k = 10. <strong>(25 points)</strong>




<ol>

 <li>K-means clustering (implemented in Problem 1).</li>

 <li>Agglomerative clustering with Ward linkage <a href="http://scikit-learn.org/stable/modules/clustering.html#hierarchical-clustering">(</a><a href="http://scikit-learn.org/stable/modules/clustering.html#hierarchical-clustering">cluster.AgglomerativeClustering</a><a href="http://scikit-learn.org/stable/modules/clustering.html#hierarchical-clustering">)</a>.</li>

 <li>Affinity Propagation <a href="http://scikit-learn.org/stable/modules/clustering.html#affinity-propagation">(</a><a href="http://scikit-learn.org/stable/modules/clustering.html#affinity-propagation">cluster.AffinityPropagation</a><a href="http://scikit-learn.org/stable/modules/clustering.html#affinity-propagation">)</a>.</li>

</ol>




The dataset you will be working with is the handwritten digits and the details can be found <a href="http://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_digits.html">here</a><a href="http://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_digits.html">.</a>




<strong><em>Assess all three clustering algorithms using the following protocol: </em></strong>




<ol>

 <li>Each cluster should be defined by the digit that represents <em>the majority</em> of the current cluster. For examples, if in the second cluster, there are 60 data points of digit “5”, 40 of “3” and 25 of</li>

</ol>

“2”, the cluster is labeled as “5”.




<ol>

 <li>Report the 10×10 confusion matrix by comparing the predicted clusters with the actual labels of the datasets. If the clustering procedure resulted in less than 10 clusters, output “-1” in the position to the missing clusters in the confusion matrix.</li>

</ol>




<ul>

 <li>Calculate the accuracy of each clustering method using the <a href="https://en.wikipedia.org/wiki/Fowlkes%E2%80%93Mallows_index">Fowlkes</a><a href="https://en.wikipedia.org/wiki/Fowlkes%E2%80%93Mallows_index">–</a><a href="https://en.wikipedia.org/wiki/Fowlkes%E2%80%93Mallows_index">Mallows index</a> <a href="http://scikit-learn.org/stable/modules/clustering.html#fowlkes-mallows-scores">(</a><a href="http://scikit-learn.org/stable/modules/clustering.html#fowlkes-mallows-scores">metrics.fowlkes_mallows_score</a><a href="http://scikit-learn.org/stable/modules/clustering.html#fowlkes-mallows-scores">)</a>.</li>

</ul>




<strong> </strong>

<h1>Problem 4</h1>




Apply three classification algorithms to the same <strong>ckd_data.zip</strong> dataset as in Problem 2. <strong>(15 points)</strong>




<ol>

 <li>Support Vector Machine with the linear kernel and default parameters <a href="http://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html">(</a><a href="http://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html">svm.SVC</a><a href="http://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html">)</a>.</li>

 <li>Support Vector Machine with the RBF kernel and default parameters.</li>

 <li>Random forest with default parameters <a href="http://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html">(</a><a href="http://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html">ensemble.RandomForestClassifier</a><a href="http://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html">)</a>.</li>

</ol>




<strong><em>Assess all three classification algorithms using the following protocol: </em></strong>




<ol>

 <li>Use 80% of each class data to train your classifier and the remaining 20% to test it.</li>

 <li>Report the f-measure of the algorithm’s performance on the <strong>training and test sets.</strong></li>

</ol>




<em>f -measure</em>= 2<em>Pre</em><em>Rec Pre</em>+ <em>Rec</em>

<h2>                                                                   TP                      TP</h2>

where <em>Pre</em>= ;        <em>Rec</em>=    ; <em>TP </em>+ <em>FP        TP </em>+ <em>FN</em>


