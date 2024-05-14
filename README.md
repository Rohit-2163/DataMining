# DataMining

## Practical List
The practicals are to be performed on R or Python. The operations are to be performed on 
downloadable datasets mentioned in references below.
<div>Section 1: Preprocessing</div><br>
<h2>Q1. Create a file “people.txt” with the following data:</h2><br>

<table>
    <tr>
        <th>Age</th>
        <th>agegroup</th>
        <th>height</th>
        <th>status</th>
        <th>yearsmarried</th>
    </tr>
    <tr>
        <td>21</td>
        <td>adult</td>
        <td>6.0</td>
        <td>single</td>
        <td>-1</td>
    </tr>
    <tr>
        <td>2</td>
        <td>child</td>
        <td>3</td>
        <td>married</td>
        <td>0</td>
    </tr>
    <tr>
        <td>18</td>
        <td>adult</td>
        <td>5.7</td>
        <td>married</td>
        <td>20</td>
    </tr>
    <tr>
        <td>221</td>
        <td>elderly</td>
        <td>5</td>
        <td>widowed</td>
        <td>2</td>
    </tr>
    <tr>
        <td>34</td>
        <td>child</td>
        <td>-7</td>
        <td>married</td>
        <td>3</td>
    </tr>
</table>

<ol>
    <li>Read the data from the file “people.txt”.</li>
    <li>Create a ruleset E that contain rules to check for the following conditions:
        <ol type="a">
            <li>The age should be in the range 0-150.</li>
            <li>The age should be greater than yearsmarried.</li>
            <li>The status should be married or single or widowed.</li>
            <li>If age is less than 18 the agegroup should be child, if age is between 18 and 65 the agegroup should be adult, if age is more than 65 the agegroup should be elderly.</li>
        </ol>
    </li>
    <li>Check whether ruleset E is violated by the data in the file people.txt.</li>
    <li>Summarize the results obtained in part (iii)</li>
    <li>Visualize the results obtained in part (iii)</li>
</ol>

<h2>Q2. Perform the following preprocessing tasks on the dirty_iris datasetii.</h2>
<ol>
    <li>Calculate the number and percentage of observations that are complete.</li>
    <li>Replace all the special values in data with NA.</li>
    <li>Define these rules in a separate text file and read them. (Use editfile function in R (package editrules). Use similar function in Python). Print the resulting constraint object.
        <ol type="a">
            <li>Species should be one of the following values: setosa, versicolor or virginica.</li>
            <li>All measured numerical properties of an iris should be positive.</li>
            <li>The petal length of an iris is at least 2 times its petal width.</li>
            <li>The sepal length of an iris cannot exceed 30 cm.</li>
            <li>The sepals of an iris are longer than its petals.</li>
        </ol>
    </li>
    <li>Determine how often each rule is broken (violatedEdits). Also summarize and plot the result.</li>
    <li>Find outliers in sepal length using boxplot and boxplot.stats</li>
</ol>


<h2>Q3. Load the data from wine dataset. Check whether all attributes are standardized or not (mean 
is 0 and standard deviation is 1). If not, standardize the attributes. Do the same with Iris dataset.<h2>

<br><br>
<h1>Section 2: Data Mining Techniques</h1>
<h2>Run following algorithms on 2 real datasets and use appropriate evaluation measures to compute 
correctness of obtained patterns:</h2>
<h2>Q4. Run Apriori algorithm to find frequent itemsets and association rules</h2>
<ol>
  <li>Use minimum support as 50% and minimum confidence as 75%</li>
  <li>Use minimum support as 60% and minimum confidence as 60%</li>
</ol>

<h2>Q5. Use Naive bayes, K-nearest, and Decision tree classification algorithms and build classifiers. 
Divide the data set into training and test set. Compare the accuracy of the different classifiers 
under the following situations:</h2>
<ol>
  <li>
    <p>a) Training set = 75%, Test set = 25%</p>
    <p>b) Training set = 66.6% (2/3rd of total), Test set = 33.3%</p>
  </li>
  <li>
    Training set is chosen by 
    <ol type="i">
      <li>hold out method</li>
      <li>Random subsampling</li>
      <li>Cross-Validation</li>
    </ol>
    Compare the accuracy of the classifiers obtained.
  </li>
  <li>Data is scaled to standard format.</li>
</ol>


<h2>Q6. Use Simple Kmeans, DBScan, Hierachical clustering algorithms for clustering. Compare the 
performance of clusters by changing the parameters involved in the algorithms.</h2><br><br
