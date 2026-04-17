<h1>Embedding</h1>

<h2>Description</h2>

<p>Adds the weight of the Embedding layer to the weights table. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="Embedding" src="assets/Embedding.png" width="258"/></p>

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
      <td valign="top"><strong>embeddings : <em>array, </em></strong>2D values. embeddings = [input_dim, output_dim].</td>
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
<li>embeddings = [input_dim, output_dim]</li>
</ul>

<p>The size depends on the input_dim and output_dim parameters of the <a href="../../../../architecture/layers/embedding-add-to-graph/README.md">Embedding</a> layer.<br/>For example if the input_dim parameter has the value 5 and the output_dim parameter has the value 3 then the size of embeddings will be [input_dim = 5, output_dim = 3].</p>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>
