<h1>SpecificityAtSensitivity</h1>

<h2>Description</h2>

<p>Computes best specificity where sensitivity is &gt; specified value. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="specificity_at_sensitivity.png" src="assets/specificity_at_sensitivity.png" width="460"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Array Single.Png" src="assets/array-single.png" width="42"/></td>
      <td valign="top"><strong>y_pred : <em>array, </em></strong>predicted values.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Array Single.Png" src="assets/array-single.png" width="42"/></td>
      <td valign="top"><strong>y_true : <em>array, </em></strong>true values.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Single.Png" src="assets/single.png" width="42"/></td>
      <td valign="top"><strong> sensitivity : <em>float,</em></strong> a scalar value in range [0 ,1].</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Integer 32.Png" src="assets/integer-32.png" width="42"/></td>
      <td valign="top"><strong>num_thresholds</strong><em><strong> : integer</strong><strong>,</strong></em> the number of thresholds to use for matching the given recall.</td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Out Single.Png" src="assets/out-single.png" width="42"/></td>
      <td valign="top"><strong>specificity</strong><strong>_at_sensitivity : <em>float, </em></strong>result.</td>
    </tr>
  </tbody>
</table>

<h2>Calculation</h2>

<p>The SpecificityAtSensitivity metric is used to evaluate the performance of classification models. It calculates specificity, i.e. the ratio of true negatives to the sum of true negatives and false positives, at a specified sensitivity level. Sensitivity is the ratio of true positives to the sum of true positives and false negatives.<br/>To calculate this metric, a number of thresholds (num_thresholds) are used. For each threshold, calculated as i / (num_thresholds – 1) where i ranges from 0 to num_thresholds, specificity and sensitivity are calculated.<br/>Then, when sensitivity reaches or exceeds the specified value (sensitivity), the highest specificity obtained among all the thresholds is retained.</p>

<p>This metric offers a balance between specificity and sensitivity.</p>

<table>
  <tbody>
    <tr>
      <td valign="top" width="50%"><p align="center"><img alt="specificity_calcul" src="assets/specificity_calcul.png" width="220"/></p></td>
      <td valign="top" width="50%"><p align="center"><img alt="sensitivity_calcul" src="assets/sensitivity_calcul.png" width="220"/></p></td>
    </tr>
  </tbody>
</table>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>

<h3>Easy to use</h3>

<p align="center"><img alt="SpecificityAtSensitivity" src="assets/specificity_at_sensitivity.png" width="220"/></p>
