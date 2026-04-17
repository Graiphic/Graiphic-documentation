<h1>CategoricalHinge</h1>

<h2>Description</h2>

<p>Computes the categorical hinge metric between y_true and y_pred. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="CategoricalHinge" src="assets/CategoricalHinge.png" width="460"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Array Single.Png" src="assets/array-single.png" width="42"/></td>
      <td valign="top"><strong>y_pred : <em>array, </em></strong>predicted values (one hot probabilities for example, [0.1, 0.3, 0.6] for 3-class problem).</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Array Single.Png" src="assets/array-single.png" width="42"/></td>
      <td valign="top"><strong>y_true : <em>array, </em></strong>true values (one hot for example, [0, 0, 1] for 3-class problem).</td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Out Single.Png" src="assets/out-single.png" width="42"/></td>
      <td valign="top"><strong>categorical_hinge : <em>float, </em></strong>result.</td>
    </tr>
  </tbody>
</table>

<h2>Use cases</h2>

<p>The categorical hinge metric, also known as categorical margin loss, is a loss function used in machine learning for multiclass classification problems. For example, it could be used to train a model to classify images into different categories (such as different types of clothing) or to classify text documents into different genres. This metric is often used in the fields of computer vision and natural language processing, but can be applied to any multiclass classification task.</p>

<h2>Calculation</h2>

<p>The function calculates the difference between the true class and the predicted value, then takes the maximum between this difference and 0.</p>

<p>If the prediction is correct (if y_pred is equal to y_true), then the loss value is 0. If the prediction is incorrect, the loss value is the difference between the true class and the prediction.</p>

<p align="center"><img alt="categorical_hinge_calcul" src="assets/categorical_hinge_calcul.png" width="220"/></p>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>

<h3>Easy to use</h3>

<p align="center"><img alt="CategoricalHinge" src="assets/categorical_hinge.png" width="220"/></p>
