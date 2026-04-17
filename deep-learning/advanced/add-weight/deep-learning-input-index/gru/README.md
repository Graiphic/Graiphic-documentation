<h1>GRU</h1>

<h2>Description</h2>

<p>Adds the weights of the GRU layer to the weights table. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="GRU" src="assets/GRU.png" width="295"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td valign="top" width="70%"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Cluster Array In.Png" src="assets/cluster-array-in.png" width="42"/></td>
      <td valign="top"><strong>Weights in : array</strong></td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Integer 32.Png" src="assets/integer-32.png" width="42"/></td>
      <td valign="top"><strong>index : <em>integer,</em></strong> index of layer.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="var-in.png" src="assets/var-in.png" width="42"/></td>
      <td valign="top"><strong>weights : <em>variant,</em></strong> weights values.</td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img alt="weights_in_by_index" src="assets/weights_in_by_index.png" width="220"/></p></td>
    </tr>
  </tbody>
</table>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Integer 32.Png" src="assets/integer-32.png" width="42"/></td>
      <td valign="top"><strong>index : <em>integer</em>, </strong>index of layer.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Array Single.Png" src="assets/array-single.png" width="42"/></td>
      <td valign="top"><strong>input_weights : <em>array, </em></strong>2D values. input_weights = [features, 3*units].</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Array Single.Png" src="assets/array-single.png" width="42"/></td>
      <td valign="top"><strong>hidden_weights : <em>array, </em></strong>2D values. hidden_weights = [units, 3*units].</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Array Single.Png" src="assets/array-single.png" width="42"/></td>
      <td valign="top"><strong>input_biases : <em>array, </em></strong>1D values. input_biases = [3*units].</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Array Single.Png" src="assets/array-single.png" width="42"/></td>
      <td valign="top"><strong>hidden_biases : <em>array, </em></strong>1D values. hidden_biases = [3*units].</td>
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
      <td width="64" valign="top"><img alt="Cluster Array Out.Png" src="assets/cluster-array-out.png" width="42"/></td>
      <td valign="top"><strong>Weights out : array</strong></td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Integer 32 Out.Png" src="assets/integer-32-out.png" width="42"/></td>
      <td valign="top"><strong>index : <em>integer,</em></strong> index of layer.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="var-out.png" src="assets/var-out.png" width="42"/></td>
      <td valign="top"><strong>weights : <em>variant,</em></strong> weights values.</td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img alt="weights_out_by_index" src="assets/weights_out_by_index.png" width="220"/></p></td>
    </tr>
  </tbody>
</table>

<h2>Dimension</h2>

<ul>
<li>input_weights = [features, 3*units]</li>
</ul>

<p>The size depends on the <a href="../../../../architecture/layers/gru-add-to-graph/README.md">GRU</a> layer input and the units parameter.<br/>For example, if the input has a size of [batch = 10, timesteps = 8, features = 5] and units a value of 3 then input_weights will have a size of [features = 5, 3*units = 3].<br/>Another example, if the input has a size of [batch = 15, timesteps = 8, features = 6] and units a value of 2 then input_weights will have a size of [features = 6, 3*units = 2].</p>

<ul>
<li>hidden_weights = [units, 3*units].</li>
</ul>

<p>The size depends on the units parameter of the <a href="../../../../architecture/layers/gru-add-to-graph/README.md">GRU</a> layer.<br/>For example, if units has a value of 6 then hidden_weights will have a size of [units = 6, 3*units = 6].<br/>Another example, if units has a value of 4 then hidden_weights will have a size of [units = 4, 3*units = 4].</p>

<ul>
<li>input_biases = [3*units]</li>
</ul>

<p>The size depends on the units parameter of the <a href="../../../../architecture/layers/gru-add-to-graph/README.md">GRU</a> layer.<br/>For example, if units has a value of 6, then input_biases will have a size of [3*units = 6].<br/>Another example, if units has a value of 4, then input_biases will have a size of [3*units = 4].</p>

<ul>
<li>hidden_biases = [3*units]</li>
</ul>

<p>The size of hidden_biases is based on the same principle as the size of input_biases.</p>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>
