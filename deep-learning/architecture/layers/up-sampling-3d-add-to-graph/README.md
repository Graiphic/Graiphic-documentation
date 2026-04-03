<h1>UpSampling3D</h1>

<h2>Description</h2>

<p>Setup and add the up sampling 3D layer into the model during the definition graph step. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img src="assets/up_sampling_3d_add_to_graph.png" alt="Up_Sampling_3D_Add_To_Graph.Png" width="262" /></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Model.Png" src="assets/input_model.png" width="42"/></td>
      <td valign="top"><strong>Model in : </strong>model architecture.</td>
    </tr>
  </tbody>
</table>

<table>
  <tbody>
    <tr>
      <td valign="top" width="75%"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Cluster.Png" src="../../../../_resolved/and/assets/cluster.png" width="42"/></td>
      <td valign="top"><strong>Parameters :</strong> layer parameters.</td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Out Array Integer 32.Png" src="assets/out-array-integer-32.png" width="42"/></td>
      <td valign="top"><strong>size : <em>array integers</em></strong>, the upsampling factors for dim1, dim2 and dim3.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “[2,2,2]”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Array_Enum.Png" src="assets/output_array_enum.png" width="42"/></td>
      <td valign="top"><strong>data format : <em>enum</em></strong>, one of <strong>channels_last</strong> or <strong>channels_first</strong> (default) . The ordering of the dimensions in the inputs. <strong>channels_last</strong> corresponds to inputs with shape <strong>(batch, height, width, channels)</strong> while <strong>channels_first </strong>corresponds to inputs with shape <strong>(batch, channels, height, width)</strong>.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “channels_first”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Booleen.Png" src="assets/booleen.png" width="42"/></td>
      <td valign="top"><strong>training? :</strong> <em><strong>boolean</strong></em>, whether the layer is in training mode (can store data for backward).</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “True”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Array_Double.Png" src="assets/input_array_double.png" width="42"/></td>
      <td valign="top"><strong>lda coeff :</strong> <em><strong>float</strong></em>, defines the coefficient by which the loss derivative will be multiplied before being sent to the previous layer (since during the backward run we go backwards).</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “1”.</td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="25%"><p align="center"><img src="assets/param_upsampling_3d.png" alt="param_upsampling_3d" width="106" /></p></td>
    </tr>
  </tbody>
</table>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Array_String.Png" src="assets/input_array_string.png" width="42"/></td>
      <td valign="top"><strong>name (optional) :</strong> <em><strong>string,</strong></em> name of the layer.</td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Model.Png" src="assets/output_model.png" width="42"/></td>
      <td valign="top"><strong>Model out : </strong>model architecture.</td>
    </tr>
  </tbody>
</table>

<h2>Dimension</h2>

<h3>Input shape</h3>

<p>5D tensor with shape :</p>

<ul>
<li>If data_format = ‘channels_last’ : (batch_size, dim1, dim2, dim3, channels).</li>
<li>If data_format = ‘channels_first’ : (batch_size, channels, dim1, dim2, dim3).</li>
</ul>

<h3>Output shape</h3>

<p>5D tensor with shape :</p>

<ul>
<li>If data_format = ‘channels_last’ : (batch_size, upsampled_dim1, upsampled_dim2, upsampled_dim3, channels).</li>
<li>If data_format = ‘channels_first’ : (batch_size, channels, upsampled_dim1, upsampled_dim2, upsampled_dim3).</li>
</ul>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>

<h3>UpSampling3D layer</h3>

<p align="center"><img src="assets/1-upsampling3d-layer.png" alt="1 - UpSampling3D layer" width="260" /></p>

<p>1 – Generate a set of data</p>

<p>We generate an array of data of type single and shape [batch_size = 10, channels = 7, dim1 = 5, dim2 = 5, dim3 = 3].</p>

<p>2 – Define graph</p>

<p>First, we define the first layer of the graph which is an Input layer (explicit input layer method). This layer is setup as an input array shaped [channels = 7, dim1 = 5, dim2 = 5, dim3 = 3].<br/>Then we add to the graph the UpSampling3D layer.</p>

<p>3 – Run graph</p>

<p>We call the forward method and retrieve the result with the “Prediction 5D” method.<br/>This method returns two variables, the first one is the layer information (cluster composed of the layer name, the graph index and the shape of the output layer) and the second one is the prediction with a shape of [batch_size, channels, upsampled_dim1, upsampled_dim2, upsampled_dim3].</p>

<h3>UpSampling3D layer, batch and dimension</h3>

<p align="center"><img src="assets/2-upsampling3d-batch-and-dimension.png" alt="2 - Upsampling3D batch and dimension" width="260" /></p>

<p>1 – Generate a set of data</p>

<p>We generate an array of data of type single and shape [numberof batch = 9, batch_size = 10, channels = 7, dim1 = 5, dim2 = 5, dim3 = 3].</p>

<p>2 – Define graph</p>

<p>First, we define the first layer of the graph which is an Input layer (explicit input layer method). This layer is setup as an input array shaped [channels = 7, dim1 = 5, dim2 = 5, dim3 = 3].<br/>Then we add to the graph the UpSampling3D layer.</p>

<p>3 – Run graph</p>

<p>We call the forward method and retrieve the result with the “Prediction 5D” method.<br/>This method returns two variables, the first one is the layer information (cluster composed of the layer name, the graph index and the shape of the output layer) and the second one is the prediction with a shape of [batch_size, channels, upsampled_dim1, upsampled_dim2, upsampled_dim3].</p>
