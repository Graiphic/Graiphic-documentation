<h1>Custom</h1>

<h2>Description</h2>

<p>A custom loss function allows you to define your own loss logic, making it possible to go beyond the standard loss functions provided by libraries. Instead of being limited to the default losses (e.g., Binary Crossentropy, MSE), you can create a custom loss by combining existing operations or designing a new formula that better suits your task. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="enum.png" src="assets/enum.png" width="209"/></p>

<p>However, custom loss functions can also accept additional arguments if needed, for example, class weights, auxiliary data, or even internal model states. This makes it possible to build more sophisticated loss strategies, including :</p>

<ul>
<li>Modifying an existing loss (e.g., adding regularization or a masking condition)</li>
<li>Designing <strong>multi-input</strong> losses (e.g., for Siamese or triplet networks)</li>
<li>Combining multiple objectives (e.g., reconstruction + classification)</li>
<li>Integrating domain-specific rules directly into the training signal</li>
</ul>

<p>The custom loss must be provided as a valid ONNX model. This model must follow two rules :  </p>

<ul>
<li>It must have an input named “prediction”, which will receive the output of the network during training.  </li>
<li>It must have a single scalar output, representing the computed loss value. </li>
</ul>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Model.Png" src="assets/input_model.png" width="42"/></td>
      <td valign="top"><strong>Model in : </strong>model architecture.</td>
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
      <td width="64" valign="top"><img alt="custom_loss.png" src="assets/custom_loss.png" width="42"/></td>
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
      <td valign="top"><strong>y_pred : <em>array,</em></strong> the model’s predictions.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Array Single.Png" src="assets/array-single.png" width="42"/></td>
      <td valign="top"><strong>y_true : <em>array, </em></strong>the ground truth data.</td>
    </tr>
  </tbody>
</table>

<h2>Use cases</h2>

<p>Custom losses are especially valuable when your performance metric is complex, composite, or cannot be captured by standard loss functions. By enabling fine control over the optimization target, they ensure the training process is aligned with the true goal of your application.</p>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>

<p align="center"><img alt="loss_exemple" src="assets/loss_exemple.png" width="220"/></p>
