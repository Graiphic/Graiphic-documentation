<h1>L1</h1>

<h2>Description</h2>

<p>Define L2 regularizer. L2 regularization applies a penalty proportional to the <strong>square of the weights</strong>. It discourages large weight values and helps improve <strong>generalization</strong> by smoothing the model. When selected explicitly, the <strong><code>l2</code> coefficient is user-defined</strong>, while <code>l1</code> is ignored. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="L2" src="assets/L2.png" width="221"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Single.Png" src="assets/single.png" width="42"/></td>
      <td valign="top"><strong>l2 : <em>float, </em></strong>L2 regularization factor.</td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td valign="top" width="75%"><p><img alt="Cluster Out.Png" src="assets/cluster-out.png" width="32"/><strong>Regularizer :</strong><em><strong>cluster,</strong></em>this cluster defines the regularization strategy used to constrain model weights.</p>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="output_object.png" src="assets/output_object.png" width="42"/></td>
      <td valign="top"><strong><a href="../../../../more-deep-learning/layers-parameters/regularizer/README.md">enum</a> :</strong> <em><strong>enum</strong></em>, an enumeration indicating the regularizer type (e.g., None, L1, L2, etc.). If <code>enum</code> is set to <code>CustomRegularizer</code>, the custom class will be used. Otherwise, the selected regularizer will be applied using default settings.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="l2.png" src="assets/l2.png" width="42"/></td>
      <td valign="top"><strong>Class :</strong> <em><strong>object</strong></em>, a custom regularizer class instance.</td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="25%"><p align="center"><img alt="output_regularizer" src="assets/output_regularizer.png" width="220"/></p></td>
    </tr>
  </tbody>
</table>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>

<p align="center"><img alt="regularizer_exemple" src="assets/regularizer_exemple.png" width="220"/></p>
