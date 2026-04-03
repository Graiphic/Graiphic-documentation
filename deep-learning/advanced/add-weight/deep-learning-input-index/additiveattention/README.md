<h1>AdditiveAttention</h1>

<h2>Description</h2>

<p>Adds the weight of the AdditiveAttention layer to the weights table. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="additive_attention_format_by_index.PNG" src="assets/additive_attention_format_by_index.PNG" width="243"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td valign="top" width="70%"><p><img alt="Cluster Array In.Png" src="assets/cluster-array-in.png" width="32"/><strong>Weights in : array</strong></p>

<table>
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
      <td valign="top" width="30%"><p align="center"><img alt="weights_in_by_index" src="assets/weights_in_by_index.png" width="220"/></p></td>
    </tr>
  </tbody>
</table>

<p><img alt="Integer 32.Png" src="assets/integer-32.png" width="32"/><strong>index : <em>integer</em>, </strong>index of layer.<br/><img alt="Array Single.Png" src="assets/array-single.png" width="32"/><strong>scale : <em>array, </em></strong>1D values. scale = query[2] = value[2] = key[2].</p>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td valign="top" width="70%"><p><img alt="Cluster Array Out.Png" src="assets/cluster-array-out.png" width="32"/><strong>Weights out : array</strong></p>

<table>
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
      <td valign="top" width="30%"><p align="center"><img alt="weights_out_by_index" src="assets/weights_out_by_index.png" width="220"/></p></td>
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
