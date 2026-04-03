<h1>ConvLSTM1D</h1>

<h2>Description</h2>

<p>Returns the ConvLSTM1D layer weights. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="conv_lstm_1d_format.png" src="assets/conv_lstm_1d_format.png" width="233"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td valign="top" width="70%"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Cluster.Png" src="assets/cluster.png" width="42"/></td>
      <td valign="top"><strong>weights : cluster</strong></td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Integer 32.Png" src="assets/integer-32.png" width="42"/></td>
      <td valign="top"><strong>index : <em>integer, </em></strong>index of layer.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="String.Png" src="assets/string.png" width="42"/></td>
      <td valign="top"><strong>name : <em>string, </em></strong>name of layer.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="var-in.png" src="assets/var-in.png" width="42"/></td>
      <td valign="top"><strong>weight : <em>variant, </em></strong>weight of layer.</td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img alt="input_weight_format" src="assets/input_weight_format.png" width="220"/></p></td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td valign="top" width="70%"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Cluster Out.Png" src="assets/cluster-out.png" width="42"/></td>
      <td valign="top"><strong>weights_info : cluster</strong></td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Integer 32 Out.Png" src="assets/integer-32-out.png" width="42"/></td>
      <td valign="top"><strong>index : <em>integer, </em></strong>index of layer.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="String Out.Png" src="assets/string-out.png" width="42"/></td>
      <td valign="top"><strong>name : <em>string, </em></strong>name of layer.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Cluster Out.Png" src="assets/cluster-out.png" width="42"/></td>
      <td valign="top"><strong>weights : cluster</strong></td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Array Single Out.Png" src="assets/array-single-out.png" width="42"/></td>
      <td valign="top"><strong>kernel : <em>array, </em></strong>3D values. kernel = [4*n_filters, channels, size].</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Array Single Out.Png" src="assets/array-single-out.png" width="42"/></td>
      <td valign="top"><strong>recurrent_kernel : <em>array, </em></strong>3D values. recurrent_kernel = [4*n_filters, n_filters, size].</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Array Single Out.Png" src="assets/array-single-out.png" width="42"/></td>
      <td valign="top"><strong>bias : <em>array, </em></strong>1D values. bias = [4*n_filters].</td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img alt="conv_lstm_1d_weights_info" src="assets/conv_lstm_1d_weights_info.png" width="220"/></p></td>
    </tr>
  </tbody>
</table>

<h2>Dimension</h2>

<ul>
<li>kernel = [4*n_filters, channels, size]</li>
</ul>

<p>The kernel size depends on the input of the <a href="../../../architecture/layers/conv-lstm-1d-add-to-graph/README.md">ConvLSTM1D</a> layer and the parameters n_filters and size of the ConvLSTM1D cell.<br/>
For example, if the input of the layer has a size of [samples = 10, time = 8, channels = 5, rows = 2], n_filters a value of 6 and size the value 3, then kernel will have a size of [4*n_filters = 6, channels = 5, size = 3].</p>

<ul>
<li>recurrent_kernel = [4*n_filters, n_filters, size].</li>
</ul>

<p>The size of recurrent_kernel depends on the parameters n_filters and size of the ConvLSTM1D cell.<br/>
For example, if n_filters has a value of 6 and size the value 3, then recurrent_kernel will have a size of [4*n_filters = 6, n_filters = 6, size = 3].</p>

<ul>
<li>bias = [4*n_filters].</li>
</ul>

<p>The size of bias depends on the parameter n_filters of the ConvLSTM1D cell.<br/>
For example, if n_filters has a value of 6 then the bias size will be [4*n_filters = 6].</p>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>
