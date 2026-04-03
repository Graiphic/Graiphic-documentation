<h1>Convolution 3D</h1>

<h2>Description</h2>

<p>Defines the weights of the Conv3D layer selected by the name. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img src="assets/set_weights_conv_3d_name.png" alt="Set_Weights_Conv_3D_Name.Png" width="228" /></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Model.Png" src="assets/input_model.png" width="42"/></td>
      <td valign="top"><strong>Model in : </strong>model architecture.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="String.Png" src="assets/string.png" width="42"/></td>
      <td valign="top"><strong>name : <em>string</em>, </strong>name of layer.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Array Single.Png" src="assets/array-single.png" width="42"/></td>
      <td valign="top"><strong>filters : <em>array, </em></strong>5D values. filters = [n_filters, channel, size[0], size[1], size[2]].</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Array Single.Png" src="assets/array-single.png" width="42"/></td>
      <td valign="top"><strong>biases : <em>array, </em></strong>1D values. biases = [n_filters].</td>
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
<li>filters = [n_filters, channel, size[0], size[1], size[2]]</li>
</ul>

<p>The size of filters depends on the input of the <a href="../../../../architecture/layers/conv-3d-add-to-graph/README.md">Conv3D</a> layer and the parameters n_filters and size.<br/>For example, if the input of the layer has a size of [batch_size = 10, channel = 8, conv_dim1 = 7, conv_dim2 = 5, conv_dim3 = 5], n_filters has the value 6 and size the value [3, 3, 3] then filters will have a size of [n_filters = 6, channel = 8, size[0] = 3, size[1] = 3, size[2] = 3].</p>

<ul>
<li>biases = [n_filters].</li>
</ul>

<p>The size of biases depends on the parameter n_filters of the <a href="../../../../architecture/layers/conv-3d-add-to-graph/README.md">Conv3D</a> layer.</p>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>
