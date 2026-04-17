<h1>Dense</h1>

<h2>Description</h2>

<p>Defines the weights of the Dense layer selected by the index. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="Dense" src="assets/Dense.png" width="228"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Model.Png" src="assets/input_model.png" width="42"/></td>
      <td valign="top"><strong>Model in : </strong>model architecture.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Integer 32.Png" src="assets/integer-32.png" width="42"/></td>
      <td valign="top"><strong>index : <em>integer</em>, </strong>index of layer.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Array Single.Png" src="assets/array-single.png" width="42"/></td>
      <td valign="top"><strong>weights : <em>array, </em></strong>2D values. weights = [input_dim, units].</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Array Single.Png" src="assets/array-single.png" width="42"/></td>
      <td valign="top"><strong>biases : <em>array, </em></strong>1D values. biases = [units].</td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Model.Png" src="assets/output_model.png" width="42"/></td>
      <td valign="top"><strong>Model out : </strong>model architecture.</td>
    </tr>
  </tbody>
</table>

<h2>Dimension</h2>

<ul>
<li>weights = [input_dim, units]</li>
</ul>

<p>The size of weights depends on the input of the <a href="../../../../architecture/layers/dense-add-to-graph/README.md">Dense</a> layer and the parameters units.<br/>For example if the input of the layer has a size of [batch_size = 10, input_dim = 5] and units the value 3 then weights will have a size of [input_dim = 5, units = 3].</p>

<ul>
<li>biases = [units]</li>
</ul>

<p>The size of biases depends on the parameter units of the <a href="../../../../architecture/layers/dense-add-to-graph/README.md">Dense</a> layer.</p>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>
