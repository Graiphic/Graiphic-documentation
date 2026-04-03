<h1>AdditiveAttention</h1>

<h2>Description</h2>

<p>Gets the weights of the AdditiveAttention layer selected by the name. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img src="assets/get_weights_by_name.png" alt="Get_Weights_By_Name.Png" width="240" /></p>

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
      <td valign="top"><strong>scale : <em>array, </em></strong>1D values. scale = query[2] = value[2] = key[2].</td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img src="assets/additive_attention_weights_info.png" alt="additive_attention_weights_info" width="157" /></p></td>
    </tr>
  </tbody>
</table>

<h2>Dimension</h2>

<ul>
<li>scale = query[2] = value[2] = key[2]</li>
</ul>

<p>The size of scale depends on the size of the query, value and key entries in the <a href="../../../../architecture/layers/additive-attention-add-to-graph/README.md">AdditiveAttention</a> layer.<br/>
For example, if query has a size of [batch_size = 5<strong>,</strong> Tq = 3, dim = 1], value a size of [batch_size = 10, Tv = 4, dim = 1] and key a size of [batch_size = 8, Tv = 6, dim = 1] then the size of scale is [dim = 1].<br/>
Another example, if query has a size of [batch_size = 10, Tq = 9, dim = 5], value a size of [batch_size = 15, Tv = 10, dim = 5] and key a size of [batch_size = 9, Tv = 7, dim = 5] then the size of scale is [dim = 5].<br/>
<strong><em>query, value and key will always have the same value at index 2 of their size, which will be the size of scale.</em></strong></p>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>
