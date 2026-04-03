<h1>Convolution 3D Transpose</h1>

<h2>Description</h2>

<p>Setup and add the convolution 3D transpose layer into the model during the definition graph step. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img src="assets/conv_3d_transpose_add_to_graph.png" alt="Conv_3D_Transpose_Add_To_Graph.Png" width="265" /></p>

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
      <td valign="top"><strong>Parameters : </strong>layer parameters.</td>
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
      <td valign="top">Default value “3”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Array Integer 32.Png" src="assets/array-integer-32.png" width="42"/></td>
      <td valign="top"><strong>size :</strong> <strong>array</strong> <em><strong>integer</strong></em>, specify the depth, height and width of the 3D convolution window. Can be a single integer to specify the same value for all spatial dimensions.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “[3,3,3]”. <em><strong>Never more 3 values</strong></em></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Array Integer 32.Png" src="assets/array-integer-32.png" width="42"/></td>
      <td valign="top"><strong>stride :</strong> <strong>array</strong> <em><strong>integer</strong></em>, specify the strides of the convolution along the depth, height and width. Can be a single integer to specify the same value for all spatial dimensions.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “[1,1,1]”. <em><strong>Never more 3 values</strong></em></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Out Array Integer 32.Png" src="assets/out-array-integer-32.png" width="42"/></td>
      <td valign="top"><strong>dilation rate : </strong><em><strong>integer, </strong></em>specifying the dilation rate to use for dilated convolution.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “[1,1,1]”. <em><strong>Never more 3 values</strong></em></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Array Integer 32.Png" src="assets/array-integer-32.png" width="42"/></td>
      <td valign="top"><strong><a href="../../../more-deep-learning/layers-parameters/explicit-padding/README.md">explicit padding</a> </strong><strong>: </strong><em><strong>array, </strong></em>specifies the number of pixels to pad at the beginning and end of each spatial axis. Batch and channel axes are not padded. Only used when padding = <strong>EXPLICIT</strong>.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “empty”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Cluster.Png" src="../../../../_resolved/and/assets/cluster.png" width="42"/></td>
      <td valign="top"><strong><a href="../../../more-deep-learning/layers-parameters/activation/README.md">Activation</a> : <em>cluster, </em></strong>activation function to use.</td>
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
      <td width="64" valign="top"><img alt="Output_Array_Enum.Png" src="assets/output_array_enum.png" width="42"/></td>
      <td valign="top"><strong><a href="../../../more-deep-learning/layers-parameters/padding/README.md">padding</a> : <em>enum,</em></strong> type of padding to apply.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “VALID”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Enum.Png" src="assets/enum.png" width="42"/></td>
      <td valign="top"><strong>data format : <em>enum</em></strong>, one of <strong>channels_last</strong> or <strong>channels_first</strong> (default) . The ordering of the dimensions in the inputs. <strong>channel_last</strong> corresponds to inputs with shape <strong>(batch, steps, features)</strong> while <strong>channels_first</strong> corresponds to inputs with shape <strong>(batch, features, steps)</strong>.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “channels_first”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Cluster.Png" src="../../../../_resolved/and/assets/cluster.png" width="42"/></td>
      <td valign="top"><strong><a href="../../../more-deep-learning/layers-parameters/initializer/README.md">Filter Initializer</a> : <em>cluster, </em></strong>initializer for the convolution kernel.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Cluster.Png" src="../../../../_resolved/and/assets/cluster.png" width="42"/></td>
      <td valign="top"><strong><a href="../../../more-deep-learning/layers-parameters/initializer/README.md">Bias Initializer</a> : <em>cluster, </em></strong>initializer for the bias vector.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Cluster.Png" src="../../../../_resolved/and/assets/cluster.png" width="42"/></td>
      <td valign="top"><strong><a href="../../../more-deep-learning/layers-parameters/regularizer/README.md">Filter Regularizer</a> : <em>cluster, </em></strong>optional regularizer for the convolution kernel.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Cluster.Png" src="../../../../_resolved/and/assets/cluster.png" width="42"/></td>
      <td valign="top"><strong><a href="../../../more-deep-learning/layers-parameters/regularizer/README.md">Bias Regularizer</a> : <em>cluster, </em></strong>optional regularizer for the bias vector.</td>
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
      <td valign="top" width="25%"><p align="center"><img src="assets/conv_3d_param.png" alt="conv_3d_param" width="162" /></p></td>
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

<p>5-Dimension tensor with shape : [batch_size, channel, conv_dim1, conv_dim2, conv_dim3] (default “channel_first” parameters).<br/>In case of “channel_last” setup, forward function will input shape [batch_size, conv_dim1, conv_dim2, conv_dim3, channel].</p>

<h3>Output shape</h3>

<p>Same shape as input 5-Dimension tensor with shape : [batch_size, channel, conv_dim1, conv_dim2 , conv_dim3] (default “channel_first” parameters).<br/>In case of “channel_last” setup, forward function will input shape [batch_size, conv_dim1, conv_dim2, conv_dim3, channel].</p>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>

<h3>Convolution 3D Transpose layer</h3>

<p align="center"><img src="assets/1-conv3dtranspose-layer.png" alt="1 - Conv3DTranspose layer" width="260" /></p>

<p>1 – Generate a set of data</p>

<p>We generate an array of data of type single and shape [batch_size = 10, channel = 5, conv_dim1 = 64, conv_dim2 = 64, conv_dim3 = 3] (channel first default layer configuration).<br/>In case of channel last layer configuration, shape is [batch_size, conv_dim1, conv_dim2, conv_dim3, channel].</p>

<p>2 – Define graph</p>

<p>First, we define the first layer of the graph which is an Input layer (explicit input layer method). This layer is setup as an input array shaped [channel = 5, conv_dim1 = 64, conv_dim2 = 64, conv_dim3 = 3].<br/>Then we add to the graph the Conv3DTranspose layer.</p>

<p>3 – Run graph</p>

<p>We call the forward method and retrieve the result with the “Prediction 5D” method.<br/>This method returns two variables, the first one is the layer information (cluster composed of the layer name, the graph index and the shape of the output layer) and the second one is the prediction with a shape of [batch_size, filter, new_conv_dim1, new_conv_dim2, new_conv_dim3].</p>

<h3>Convolution 3D Transpose layer, batch and dimension</h3>

<p align="center"><img src="assets/2-conv3dtranspose-batch-and-dimension.png" alt="2 - Conv3DTranspose batch and dimension" width="260" /></p>

<p>1 – Generate a set of data</p>

<p>We generate an array of data of type single and shape [number of batch = 9, batch_size = 10, channel = 5, conv_dim1 = 64, conv_dim2 = 64, conv_dim3 = 3] (channel first default layer configuration).<br/>In case of channel last layer configuration, shape is [batch_size, conv_dim1, conv_dim2, conv_dim3, channel].</p>

<p>2 – Define graph</p>

<p>First, we define the first layer of the graph which is an Input layer (explicit input layer method). This layer is setup as an input array shaped [channel = 5, conv_dim1 = 64, conv_dim2 = 64, conv_dim3 = 3].<br/>Then we add to the graph the Conv3DTranspose layer.</p>

<p>3 – Run graph</p>

<p>We call the forward method and retrieve the result with the “Prediction 5D” method.<br/>This method returns two variables, the first one is the layer information (cluster composed of the layer name, the graph index and the shape of the output layer) and the second one is the prediction with a shape of [batch_size, filter, new_conv_dim1, new_conv_dim2, new_conv_dim3].</p>
