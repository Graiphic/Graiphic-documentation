<h1>Flatten</h1>

<h2>Description</h2>

<p>Setup and add the flatten layer into the model during the definition graph step. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img src="assets/flatten_add_to_graph.png" alt="Flatten_Add_To_Graph.Png" width="265" /></p>

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
      <td width="64" valign="top"><img alt="Output_Array_Enum.Png" src="assets/output_array_enum.png" width="42"/></td>
      <td valign="top"><strong>data format : <em>enum</em></strong>, one of <strong>channels_last</strong> or <strong>channels_first</strong> (default) . The ordering of the dimensions in the inputs. <strong>channel_last</strong> corresponds to inputs with shape <strong>(batch, steps, features)</strong> while <strong>channels_first</strong> corresponds to inputs with shape <strong>(batch, features, steps)</strong>.</td>
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
      <td valign="top" width="25%"><p align="center"><img src="assets/layer_param_data_format.png" alt="layer_param_data_format" width="106" /></p></td>
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

<p>2D tensor with shape :</p>

<ul>
<li>If data_format = ‘channels_last’ : (batch_size, input_dim).</li>
<li>If data_format = ‘channels_first’ : (batch_size, input_dim).</li>
</ul>

<p>3D tensor with shape :</p>

<ul>
<li>If data_format = ‘channels_last’ : (batch_size, steps, features).</li>
<li>If data_format = ‘channels_first’ : (batch_size, features, steps).</li>
</ul>

<p>4D tensor with shape :</p>

<ul>
<li>If data_format is “channels_last” : (batch_size, rows, cols, channels).</li>
<li>If data_format is “channels_first” : (batch_size, channels, rows, cols).</li>
</ul>

<p>5D tensor with shape :</p>

<ul>
<li>If data_format = ‘channels_last’ : (batch_size, input_dim1, input_dim2, input_dim3, channels).</li>
<li>If data_format = ‘channels_first’ : (batch_size, channels, input_dim1, input_dim2, input_dim3).</li>
</ul>

<h3>Output shape</h3>

<p>2D tensor with shape (with a 2D tensor as input) :</p>

<ul>
<li>If data_format = ‘channels_last’ : (batch_size, new_input).</li>
<li>If data_format = ‘channels_first’ : (batch_size, new_input).</li>
</ul>

<p>2D tensor with shape (with a 3D tensor as input) :</p>

<ul>
<li>If data_format = ‘channels_last’ : (batch_size, steps * features).</li>
<li>If data_format = ‘channels_first’ : (batch_size, features * steps).</li>
</ul>

<p>2D tensor with shape (with a 4D tensor as input) :</p>

<ul>
<li>If data_format is “channels_last” : (batch_size, rows * cols * channels).<br/>If data_format is “channels_first” : (batch_size, channels * rows * cols).</li>
</ul>

<p>2D tensor with shape (with a 5D tensor as input) :</p>

<ul>
<li>If data_format = ‘channels_last’ : (batch_size, input_dim1 * input_dim2 * input_dim3 * channels).</li>
<li>If data_format = ‘channels_first’ : (batch_size, channels * input_dim1 * input_dim2 * input_dim3).</li>
</ul>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>

<h3>Flatten layer</h3>

<p align="center"><img src="assets/1-flatten-layer.png" alt="1 - Flatten layer" width="260" /></p>

<p>1 – Generate a set of data</p>

<p>We generate an array of data of type single and shape [batch_size, channels, rows, cols] (channel first is default layer configuration).<br/>In case of channel last layer configuration, shape is [batch_size, rows, cols, channels].</p>

<p>2 – Define graph</p>

<p>First, we define the first layer of the graph which is an Input layer (explicit input layer method). This layer is setup as an input array shaped [channels = 7, rows = 5, cols = 3].<br/>Then we add to the graph the Flatten layer.</p>

<p>3 – Run graph</p>

<p>We call the forward method and retrieve the result with the “Prediction 2D” method.<br/>This method returns two variables, the first one is the layer information (cluster composed of the layer name, the graph index and the shape of the output layer) and the second one is the prediction with a shape of [batch_size, channels * rows * cols].</p>

<h3>Flatten layer, batch and dimension</h3>

<p align="center"><img src="assets/2-flatten-batch-and-dimension.png" alt="2 - Flatten batch and dimension" width="260" /></p>

<p>1 – Generate a set of data</p>

<p>We generate an array of data of type single and shape [number of batch, batch_size, channels, rows, cols] (channel first is default layer configuration).<br/>In case of channel last layer configuration, shape is [number of batch, batch_size, rows, cols, channels].</p>

<p>2 – Define graph</p>

<p>First, we define the first layer of the graph which is an Input layer (explicit input layer method). This layer is setup as an input array shaped [channels = 7, rows = 5, cols = 3].<br/>Then we add to the graph the Flatten layer.</p>

<p>3 – Run graph</p>

<p>We call the forward method and retrieve the result with the “Prediction 2D” method.<br/>This method returns two variables, the first one is the layer information (cluster composed of the layer name, the graph index and the shape of the output layer) and the second one is the prediction with a shape of [batch_size, channels * rows * cols].</p>
