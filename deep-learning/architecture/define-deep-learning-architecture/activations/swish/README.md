<h1>Swish</h1>

<h2>Description</h2>

<p>Define the swish layer according to its parameters. Type : <em><strong>polymorphic</strong></em>.</p>

<p align="center"><img alt="Swish" src="assets/Swish.png" width="238"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td valign="top" width="75%"><p><img alt="Cluster.Png" src="assets/cluster.png" width="32"/><strong>Parameters :</strong> layer parameters.</p>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Booleen.Png" src="assets/booleen.png" width="42"/></td>
      <td valign="top"><strong>training? :</strong> <em><strong>boolean</strong></em>, whether the layer is in training mode (can store data for backward).</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “True”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Double.Png" src="assets/double.png" width="42"/></td>
      <td valign="top"><strong>lda coeff :</strong> <em><strong>float</strong></em>, defines the coefficient by which the loss derivative will be multiplied before being sent to the previous layer (since during the backward run we go backwards).</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “1”.</td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="25%"><p align="center"><img src="assets/layer_param.png" alt="layer_param" width="220" /></p></td>
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
      <td valign="top"><strong>Activation :</strong> <em><strong>cluster,</strong></em> this cluster defines the activation function to be used in the model.</td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="enum.png" src="assets/enum.png" width="42"/></td>
      <td valign="top"><strong><a href="../../../../more-deep-learning/layers-parameters/activation/README.md">enum</a> :</strong> <em><strong>enum</strong></em>, an enumeration specifying the type of activation (e.g., ReLU, Sigmoid, etc.). If <code>enum</code> is set to <code>CustomActivation</code>, the custom class on the right will be used as the activation function. Otherwise, the selected activation from the enum will be used with its default parameters.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Object_2.Png" src="assets/output_object_2.png" width="42"/></td>
      <td valign="top"><strong>Class :</strong> <em><strong>object</strong></em>, a custom activation class instance.</td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="25%"><p align="center"><img src="assets/output_activation.png" alt="output_activation" width="220" /></p></td>
    </tr>
  </tbody>
</table>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>

<p align="center"><img src="assets/activation_exemple.png" alt="activation_exemple" width="220" /></p>
