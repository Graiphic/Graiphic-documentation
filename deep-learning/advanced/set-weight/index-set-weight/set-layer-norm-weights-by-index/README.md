<h1>LayerNormalization</h1>

<h2>Description</h2>

<p>Defines the weights of the LayerNormalization layer selected by the index. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="LayerNormalization" src="assets/LayerNormalization.png" width="228"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Model.Png" src="assets/input_model.png" width="42"/></td>
      <td valign="top"><strong>Model in : </strong>model architecture.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Integer 32.Png" src="assets/integer-32.png" width="42"/></td>
      <td valign="top"><strong>index : <em>integer</em>, </strong>index of layer.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Array Single.Png" src="assets/array-single.png" width="42"/></td>
      <td valign="top"><strong>gamma : <em>array, </em></strong>1D values. gamma = [input_dim1].</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Array Single.Png" src="assets/array-single.png" width="42"/></td>
      <td valign="top"><strong>beta : <em>array, </em></strong>1D values. beta = [input_dim1].</td>
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
<li>gamma = [input_dim1]</li>
</ul>

<p>The size depends on the input to the <a href="../../../../architecture/layers/layer-norm-add-to-graph/README.md">LayerNormalization</a> layer.<br/>For example, if the layer input has a size of [batch_size = 10, input_dim1 = 5, input_dim2 = 4, input_dim3 = 2] then gamma will have a size of [input_dim1 = 5].<br/>Another example, if the input of the layer has a size of [batch_size = 12, input_dim1 = 8, input_dim2 = 5, input_dim3 = 3] then gamma will have a size of [input_dim1 = 8].</p>

<ul>
<li>beta = [input_dim1]</li>
</ul>

<p>The beta size is based on the same principle as the gamma size.</p>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>
