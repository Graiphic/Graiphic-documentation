<h1>TrueNegatives</h1>

<h2>Description</h2>

<p>Calculates the number of true negatives. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="true_negatives.png" src="assets/true_negatives.png" width="460"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Array Single.Png" src="assets/array-single.png" width="42"/></td>
      <td valign="top"><strong>y_pred : <em>array, </em></strong>predicted values (logits values).</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Array Single.Png" src="assets/array-single.png" width="42"/></td>
      <td valign="top"><strong>y_true : <em>array, </em></strong>true values (logits values, or binary values if the threshold value is between 0 and 1).</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Single.Png" src="assets/single.png" width="42"/></td>
      <td valign="top"><strong> thresholds : <em>float,</em></strong> representing the threshold for deciding whether prediction and true values are 1 or 0 (above the threshold is true, below is false).</td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Out Single.Png" src="assets/out-single.png" width="42"/></td>
      <td valign="top"><strong>true_negatives : <em>float, </em></strong>result.</td>
    </tr>
  </tbody>
</table>

<h2>Use cases</h2>

<p>The “TrueNegatives” metric is commonly used in machine learning, particularly for binary classification tasks. This metric counts the number of true negatives, i.e. the number of samples that have been correctly classified as negative by the model.</p>

<p>Here are some examples of specific areas where “TrueNegatives” can be used :</p>

<ul>
<li>
<ul>
<li>Spam detection : as mentioned above, in spam detection, true negatives are correctly identified non-spam emails.</li>
<li>Medical diagnosis : in disease classification, a true negative would be a healthy patient correctly identified as such.</li>
<li>Fraud detection : in the financial field, a true negative would be a non-fraudulent transaction that has been correctly identified as such.</li>
</ul>
</li>
</ul>

<h2>Calculation</h2>

<p>“TrueNegatives” metric is used in the context of binary classification.</p>

<p>A “True Negative” (TN) occurs when a model correctly predicts the negative class for an example that is actually of the negative class. In other words, the model predicted that the event would not occur, and it did not.</p>

<table>
  <tbody>
    <tr>
      <td valign="top" width="62%"><p align="center"><img alt="False &amp; True" src="assets/False &amp; True.png" width="220"/></p></td>
      <td valign="top" width="38%"><p align="center"><img alt="true_negatives_calcul" src="assets/true_negatives_calcul.png" width="220"/></p></td>
    </tr>
  </tbody>
</table>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>

<h3>Easy to use</h3>

<p align="center"><img alt="TrueNegatives" src="assets/true_negatives.png" width="220"/></p>
