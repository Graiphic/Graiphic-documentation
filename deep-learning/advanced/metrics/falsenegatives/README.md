<h1>FalseNegatives</h1>

<h2>Description</h2>

<p>Calculates the number of false negatives. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="false_negatives.png" src="assets/false_negatives.png" width="460"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Array Single.Png" src="assets/array-single.png" width="42"/></td>
      <td valign="top"><strong>y_pred : <em>array, </em></strong>predicted values (logits values).</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Array Single.Png" src="assets/array-single.png" width="42"/></td>
      <td valign="top"><strong>y_true : <em>array, </em></strong>true values (logits values, or binary values if the threshold value is between 0 and 1).</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Single.Png" src="assets/single.png" width="42"/></td>
      <td valign="top"><strong> thresholds : <em>float,</em></strong> representing the threshold for deciding whether prediction and true values are 1 or 0 (above the threshold is true, below is false).</td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Out Single.Png" src="assets/out-single.png" width="42"/></td>
      <td valign="top"><strong>false_negatives : <em>float, </em></strong>result.</td>
    </tr>
  </tbody>
</table>

<h2>Use cases</h2>

<p>The false negatives metric is used in machine learning classification problems. A false negative occurs when the model incorrectly predicts the negative class for an observation that is actually positive. This metric is particularly important in areas where the consequences of an incorrect negative prediction (a false negative) are severe.</p>

<p>Here are a few examples :</p>

<ul>
<li>
<ul>
<li>In medicine : when diagnosing diseases, a false negative means that a sick person is incorrectly identified as being in good health. This can lead to a delay in treatment and potentially serious consequences for the patient.</li>
<li>In safety or quality testing : for example, if a model is used to detect defects in manufacturing parts, a false negative means that a defective part is incorrectly identified as defect-free. this can lead to defective products being shipped to customers.</li>
<li>In spam detection : A false negative means that a spam message is incorrectly identified as legitimate. This can result in unwanted messages being delivered to a user’s inbox.</li>
</ul>
</li>
</ul>

<h2>Calculation</h2>

<p>The “False Negatives” metric is used in the context of binary classification, where the possible outcomes are “Positive” (represented by 1) and “Negative” (represented by 0).</p>

<p>A “False Negative” (FN) occurs when a model incorrectly predicts the negative class for an example that is actually of the positive class. In other words, the model predicted that the event would not occur, but it actually did.</p>

<table>
  <tbody>
    <tr>
      <td valign="top" width="62%"><p align="center"><img alt="False &amp; True" src="assets/False &amp; True.png" width="220"/></p></td>
      <td valign="top" width="38%"><p align="center"><img alt="false_negatives_calcul" src="assets/false_negatives_calcul.png" width="220"/></p></td>
    </tr>
  </tbody>
</table>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>

<h3>Easy to use</h3>

<p align="center"><img alt="FalseNegatives" src="assets/false_negatives.png" width="220"/></p>
