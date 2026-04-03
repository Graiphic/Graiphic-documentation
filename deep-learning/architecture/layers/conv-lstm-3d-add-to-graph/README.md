<h1>ConvLSTM3D</h1>

<h2>Description</h2>

<p>Setup and add the convolution lstm 3D layer into the model during the definition graph step. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img src="assets/conv_lstm_3d_add_to_graph.png" alt="Conv_Lstm_3D_Add_To_Graph.Png" width="265" /></p>

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
      <td valign="top"><strong>Parameters : </strong>layer parameters.</td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Out Array Integer 32.Png" src="assets/out-array-integer-32.png" width="42"/></td>
      <td valign="top"><strong>filters :</strong> <em><strong>integer</strong></em>, the dimensionality of the output space.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “1”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Array Integer 32.Png" src="assets/array-integer-32.png" width="42"/></td>
      <td valign="top"><strong>size : <em>array integer</em></strong>, specify the dimensions of the convolution window.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “[3,3,3]”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Array Integer 32.Png" src="assets/array-integer-32.png" width="42"/></td>
      <td valign="top"><strong>stride : <em>array integer</em></strong>, specify the strides of the convolution.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “[1,1,1]”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Array Integer 32.Png" src="assets/array-integer-32.png" width="42"/></td>
      <td valign="top"><strong><a href="../../../more-deep-learning/layers-parameters/explicit-padding/README.md">explicit padding</a> : <em>array</em></strong>, specifies the number of pixels to pad at the beginning and end of each spatial axis. Batch and channel axes are not padded. Only used when padding = <strong>EXPLICIT</strong>.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “empty”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Array_Enum.Png" src="assets/output_array_enum.png" width="42"/></td>
      <td valign="top"><strong><a href="../../../more-deep-learning/layers-parameters/padding/README.md">padding</a> : <em>enum,</em></strong> type of padding to apply.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “VALID”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Cluster.Png" src="../../../../_resolved/and/assets/cluster.png" width="42"/></td>
      <td valign="top"><strong><a href="../../../more-deep-learning/layers-parameters/activation/README.md">Activation</a> : <em>cluster, </em></strong>applied to the candidate cell input. This function transforms the new information considered for updating the cell state.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Cluster.Png" src="../../../../_resolved/and/assets/cluster.png" width="42"/></td>
      <td valign="top"><strong><a href="../../../more-deep-learning/layers-parameters/activation/README.md">Recurrent Activation</a> : <em>cluster, </em></strong>applied to the input, forget, and output gates. It controls which parts of the past information are allowed to pass or be blocked.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Cluster.Png" src="../../../../_resolved/and/assets/cluster.png" width="42"/></td>
      <td valign="top"><strong><a href="../../../more-deep-learning/layers-parameters/activation/README.md">Output Activation</a> : <em>cluster, </em></strong>applied to the updated cell state before producing the visible hidden output of the LSTM at each time step.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Booleen.Png" src="assets/booleen.png" width="42"/></td>
      <td valign="top"><strong>use bias? :</strong> <em><strong>boolean</strong></em>, whether the layer uses a bias vector.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “True”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Cluster.Png" src="../../../../_resolved/and/assets/cluster.png" width="42"/></td>
      <td valign="top"><strong><a href="../../../more-deep-learning/layers-parameters/initializer/README.md">Kernel Initializer</a> : <em>cluster, </em></strong>initializer for the <code>kernel</code> weights matrix, used for the linear transformation of the inputs.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Cluster.Png" src="../../../../_resolved/and/assets/cluster.png" width="42"/></td>
      <td valign="top"><strong><a href="../../../more-deep-learning/layers-parameters/initializer/README.md">Recurrent Initializer</a> : <em>cluster, </em></strong>initializer for the <code>recurrent_kernel</code> weights matrix, used for the linear transformation of the recurrent state.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Cluster.Png" src="../../../../_resolved/and/assets/cluster.png" width="42"/></td>
      <td valign="top"><strong><a href="../../../more-deep-learning/layers-parameters/initializer/README.md">Bias Initializer</a> : <em>cluster, </em></strong>initializer for the bias vector.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Booleen.Png" src="assets/booleen.png" width="42"/></td>
      <td valign="top"><strong>unit forget bias? :</strong> <em><strong>boolean</strong></em>, If true, add 1 to the bias of the forget gate at initialization. Use in combination with <strong><a href="../../../more-deep-learning/layers-parameters/initializer/README.md">Bias Initializer</a></strong> = ‘Zeros’.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “True”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Out Single.Png" src="assets/out-single.png" width="42"/></td>
      <td valign="top"><strong>dropout : <em>float, </em></strong>between 0 and 1. Fraction of the units to drop for the linear transformation of the inputs.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Out Single.Png" src="assets/out-single.png" width="42"/></td>
      <td valign="top">recurrent dropout : <em>float, </em>between 0 and 1. Fraction of the units to drop for the linear transformation of the recurrent state.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Booleen.Png" src="assets/booleen.png" width="42"/></td>
      <td valign="top"><strong>return sequences? : <em>boolean</em></strong>, Whether to return the last output in the output sequence, or the full sequence.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “False”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Booleen.Png" src="assets/booleen.png" width="42"/></td>
      <td valign="top"><strong>stateful? : <em>boolean</em></strong>, if True, the last state for each sample at index i in a batch will be used as initial state for the sample of index i in the following batch.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “False”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Cluster.Png" src="../../../../_resolved/and/assets/cluster.png" width="42"/></td>
      <td valign="top"><strong><a href="../../../more-deep-learning/layers-parameters/regularizer/README.md">Kernel Regularizer</a> : <em>cluster, </em></strong>regularizer function applied to the <code>kernel</code> weights matrix.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Cluster.Png" src="../../../../_resolved/and/assets/cluster.png" width="42"/></td>
      <td valign="top"><strong><a href="../../../more-deep-learning/layers-parameters/regularizer/README.md">Recurrent Regularizer</a> : <em>cluster, </em></strong>regularizer function applied to the <code>recurrent_kernel</code> weights matrix.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Cluster.Png" src="../../../../_resolved/and/assets/cluster.png" width="42"/></td>
      <td valign="top"><strong><a href="../../../more-deep-learning/layers-parameters/regularizer/README.md">Bias Regularizer</a> : <em>cluster, </em></strong>regularizer function applied to the bias vector.</td>
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
      <td width="64" valign="top"><img alt="Booleen.Png" src="assets/booleen.png" width="42"/></td>
      <td valign="top"><strong>store? :</strong> <em><strong>boolean</strong></em>, whether the layer stores the last iteration gradient (accessible via the “get_gradients” function).</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “False”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Booleen.Png" src="assets/booleen.png" width="42"/></td>
      <td valign="top"><strong>update? :</strong> <em><strong>boolean</strong></em>, whether the layer’s variables should be updated during backward. Equivalent to freeze the layer.</td>
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
      <td valign="top" width="25%"><p align="center"><img src="assets/conv_lstm_3d_param.png" alt="conv_lstm_3d_param" width="162" /></p></td>
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

<p>6D tensor with shape</p>

<ul>
<li>If data_format = ‘channels_last’ : (samples, time, rows, cols, depth, channels).</li>
<li>If data_format = ‘channels_first’ : (samples, time, channels, rows, cols, depth).</li>
</ul>

<h3>Output shape</h3>

<ul>
<li>if “return_sequences” = True :</li>
</ul>

<ul>
<li>
<ul>
<li>If data_format = ‘channels_last’ : 6D tensor with shape (samples, timesteps, new_rows, new_cols, new_depth, filters).</li>
<li>If data_format = ‘channels_first’ : 6D tensor with shape (samples, timesteps, filters, new_rows, new_cols, new_depth).</li>
</ul>
</li>
</ul>

<ul>
<li>if “return_sequences” = False :</li>
</ul>

<ul>
<li>
<ul>
<li>If data_format = ‘channels_last’ : 5D tensor with shape (samples, new_rows, new_cols, new_depth, filters).</li>
<li>If data_format = ‘channels_first’ : 5D tensor with shape (samples, filters, new_rows, new_cols, new_depth).</li>
</ul>
</li>
</ul>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>

<h3>ConvLSTM3D layer</h3>

<p align="center"><img src="assets/1-convlstm3d-layer.png" alt="1 - ConvLSTM3D layer" width="260" /></p>

<p>1 – Generate a set of data</p>

<p>We generate an array of data of type single and shape [samples = 10, time = 7, channels = 6, rows = 5, cols = 5, depth = 3].</p>

<p>2 – Define graph</p>

<p>First, we define the first layer of the graph which is an Input layer (explicit input layer method). This layer is setup as an input array shaped [time = 7, channels = 6, rows = 5, cols = 5, depth = 3].<br/>Then we add to the graph the ConvLSTM3D layer.</p>

<p>3 – Run graph</p>

<p>We call the forward method and retrieve the result with the “Prediction 5D” method.<br/>This method returns two variables, the first one is the layer information (cluster composed of the layer name, the graph index and the shape of the output layer) and the second one is the prediction with a shape of [samples, filters, new_rows, new_cols, new_depth].<br/>The output dimension depends on the parameters “return-sequences” refer to the chapter “Dimension” of this documentation.</p>

<h3>ConvLSTM3D layer, batch and dimension</h3>

<p align="center"><img src="assets/2-convlstm3d-batch-and-dimension.png" alt="2 - ConvLSTM3D batch and dimension" width="260" /></p>

<p>1 – Generate a set of data</p>

<p>We generate an array of data of type single and shape [number of batch = 9, samples = 10, time = 7, channels = 6, rows = 5, cols = 5, depth = 3].</p>

<p>2 – Define graph</p>

<p>First, we define the first layer of the graph which is an Input layer (explicit input layer method). This layer is setup as an input array shaped [time = 7, channels = 6, rows = 5, cols = 5, depth = 3].<br/>Then we add to the graph the ConvLSTM3D layer.</p>

<p>3 – Run graph</p>

<p>We call the forward method and retrieve the result with the “Prediction 5D” method.<br/>This method returns two variables, the first one is the layer information (cluster composed of the layer name, the graph index and the shape of the output layer) and the second one is the prediction with a shape of [samples, filters, new_rows, new_cols, new_depth].<br/>The output dimension depends on the parameters “return-sequences” refer to the chapter “Dimension” of this documentation.</p>
