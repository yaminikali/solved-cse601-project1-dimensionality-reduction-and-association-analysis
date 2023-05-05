Download Link: https://assignmentchef.com/product/solved-cse601-project1-dimensionality-reduction-and-association-analysis
<br>
This project contains 2 parts. In the first part, you are asked to implement PCA (Principle Components Analysis) algorithm, project the high-dimensional data to 2 dimensions, and plot the 2-dimensional data points.  In the second part, you are asked to implement Apriori and association rule generation algorithms.

Each team should submit codes and a report, and give a demo via Zoom. Demo details will be released two days before the demo date on Piazza. You need to submit codes and report to departmental server before submission due time. <strong> </strong>

<strong>Part 1: Dimensionality Reduction </strong>

<strong>Dataset Description: </strong>

In this part, you are expected to conduct dimensionality reduction on three biomedical data files (<em>pca_a.txt</em>, <em>pca_b.txt</em>, <em>pca_c.txt</em>), which can be found on Piazza.




In each file, each row represents the record of a patient/sample; the last column is the disease name, and the remaining columns are features. Note that your code should be able to handle the data with different numbers of rows/columns.

<strong> </strong>

<strong>Required Tasks: </strong>

Please take the following steps:

<ol>

 <li>You can use your preferred programming language(s). You need to implement the PCA algorithm by yourself. Applying existing package(s) to conduct PCA directly <strong>will not</strong> receive any credit. If you are not sure about whether it is OK to use a certain function, please post your question on Piazza.</li>

 <li>Implement PCA and then run it on three data files (<em>txt</em>, <em>pca_b.txt</em>, <em>pca_c.txt</em>) to get the two-dimensional data points. For each dataset, draw the data points with a scatter plot, and color them according to their disease names.</li>

 <li>Apply existing packages to run SVD and t-SNE algorithms (Do not need to implement them by yourself) and get the two-dimensional data points. Visualize</li>

</ol>

the data points of the two algorithms on the three datasets in the same way as the visualization of PCA results in step 2.

<ol start="4">

 <li>Prepare your submission. Create a folder named <em>PCA</em>, in the folder you should include:

  <ol>

   <li>Report: A pdf file named as <em>pdf</em>. The report should contain:

    <ol>

     <li>Nine scatter plots from three datasets and three algorithms. Label them properly by the dataset name and algorithm name in each plot.</li>

     <li>Describe the flow of your PCA implementation briefly, and discuss the results obtained by different algorithms.</li>

    </ol></li>

   <li>A folder named <em>Code</em>, which contains all codes used in this part. Inside the folder, please have a file <em>README</em> to describe how to run your code.</li>

  </ol></li>

</ol>







<strong>Part 2: Association Analysis </strong>

<strong> </strong>

<strong>Dataset Description: </strong>

The dataset is about gene expressions (<em>association-rule-test-data.txt</em>) and can be found on Piazza. Each row stands for a patient/sample. The last column is the disease name.  For the remaining columns, they are gene expressions with values Up or Down (Binary Value). For example, the row “Down Down Down Up … AML” can be interpreted as “G1_ Down G2_ Down G3_ Down G4_Up … AML”, and AML is a disease name.




<strong>Required Tasks:</strong>

<ol>

 <li>Implement the Apriori algorithm to find all frequent itemsets. Report the number of frequent itemsets for support of 30%, 40%, 50%, 60%, and 70%, respectively.</li>

</ol>

Please see <em>Template.pdf</em> for details.

You <strong>should not </strong>directly call any existing function or package that implements Apriori.  Apriori algorithm should be implemented by yourself.  If you are not sure about whether it is OK to use a certain function, please post your question on Piazza.

<ol start="2">

 <li>Generate association rules based on the templates. The following are templates:

  <ul>

   <li>Template 1: {RULE|HEAD|BODY} HAS ({ANY|NUMBER|NONE}) OF (ITEM1, ITEM2, …, ITEMn)</li>

   <li>Template 2: SizeOf({HEAD|BODY|RULE}) ≥ NUMBER.</li>

   <li>Template 3: Any combined templates using AND or OR. For example:</li>

  </ul></li>

</ol>

BODY HAS (1) OF (Disease) AND HEAD HAS (NONE) OF (Disease)

Below is an example illustrating RULE, BODY and HEAD in the templates: Assume we obtain a <strong>RULE</strong> {G1_Up, G3_Down} → {G4_Down, G34_Up}. {G1_Up, G3_Down} is <strong>HEAD</strong> and {G4_Down, G34_Up} is <strong>BODY</strong>.

If support = 50% and confidence = 70% are given, you need to generate <strong>all the rules</strong> satisfying these requirements. In your report, you are asked to show the number of rules generated. However, in your code, you need to make sure that support and confidence can be changed to other values in new queries, and show and count the resulting rules you generate for each query. Please see <em>Template.pdf</em> for details.

<ol start="3">

 <li>Prepare your submission. Make a folder named <em>Association</em>, in the folder you should include:

  <ol>

   <li>Report: A pdf file named as <em>pdf</em>. The report should include:</li>

   <li>Describe Apriori algorithm and the flow of the association rule generation algorithm briefly. ii. The answers of aforementioned queries in required tasks 1&amp;2 (Number of frequent itemsets or generated rules).</li>

   <li>A folder named <em>Code</em>, which contains all codes used in this part. Inside the folder, please have a file <em>README</em> which describes how to run your code.</li>

  </ol></li>

</ol>








