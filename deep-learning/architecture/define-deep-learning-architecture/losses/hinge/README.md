<h1>Hinge</h1>

<h2>Description</h2>

<p>Computes the hinge loss between y_true and y_pred.​ Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="Hinge" src="assets/Hinge.png" width="230"/></p>

<table>
  <tbody>
    <tr>
      <td valign="top" width="70%"><h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Cluster.Png" src="assets/cluster.png" width="42"/></td>
      <td valign="top"><strong>Parameters : <em>cluster,</em></strong></td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Enum.Png" src="assets/enum.png" width="42"/></td>
      <td valign="top"><strong> reduction : <em>enum,</em></strong> type of reduction to apply to the loss. In almost all cases this should be “S<em>um over Batch</em>“.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Booleen.Png" src="assets/booleen.png" width="42"/></td>
      <td valign="top"><strong> sample weights : <em>boolean,</em></strong> if enabled, adds an input for weighting each sample individually.</td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img alt="param_hinge" src="assets/param_hinge.png" width="220"/></p></td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td valign="top" width="75%"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Cluster Out.Png" src="assets/cluster-out.png" width="42"/></td>
      <td valign="top"><strong>Loss :</strong> <em><strong>cluster,</strong></em> this cluster defines the loss function used for model training.</td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="loss.png" src="assets/loss.png" width="42"/></td>
      <td valign="top"><strong>enum :</strong> <em><strong>enum</strong></em>, an enumeration indicating the loss type (e.g., MSE, CrossEntropy, etc.). If <code>enum</code> is set to <code>CustomLoss</code>, the custom class on the right will be used as the loss function. Otherwise, the selected loss will be applied with its default configuration.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="output_object.png" src="assets/output_object.png" width="42"/></td>
      <td valign="top"><strong>Class :</strong> <em><strong>object</strong></em>, a custom loss class instance.</td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="25%"><p align="center"><img alt="output_loss" src="assets/output_loss.png" width="220"/></p></td>
    </tr>
  </tbody>
</table>

<h2>Required data</h2>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Array Single.Png" src="assets/array-single.png" width="42"/></td>
      <td valign="top"><strong>y_pred : <em>array, </em></strong>predicted values.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Array Single.Png" src="assets/array-single.png" width="42"/></td>
      <td valign="top"><strong>y_true : <em>array, </em></strong>true values are expected to be -1 or 1. If binary (0 or 1) labels are provided we will convert them to -1 or 1.</td>
    </tr>
  </tbody>
</table>

<h2>Use cases</h2>

<p>Hinge loss is a loss function primarily used in binary classification tasks, such as detecting the presence or absence of an object.</p>

<p>This function aims to maximize the margin between prediction categories. It is widely used in Support Vector Machines (SVM) because it pushes the model to not only be correct, but to be confident in its prediction with a clear margin between classes.</p>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>

<p align="center"><img alt="loss_exemple" src="assets/loss_exemple.png" width="220"/></p>
