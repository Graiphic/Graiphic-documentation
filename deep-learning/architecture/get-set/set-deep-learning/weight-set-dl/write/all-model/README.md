<h1>Load all weights model</h1>

<h2>Description</h2>

<p>Load the weights of a model. By default, all layer weights will be loaded but if you set “RANDOM” to a specific index in “init_weight_array”, the selected layer will be randomly initialized.</p>

<p align="center"><img alt="All (Model)" src="assets/All (Model).png" width="220"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Model.Png" src="assets/input_model.png" width="42"/></td>
      <td valign="top"><strong>Model in : </strong>model architecture.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Model.Png" src="assets/input_model.png" width="42"/></td>
      <td valign="top"><strong>weights_model : </strong>model architecture.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Enum.Png" src="assets/enum.png" width="42"/></td>
      <td valign="top"><strong>file_type : <em>enum</em>,</strong> type of the file on which the summary is written.
<ul>
<li>
<ul>
<li><strong>None :</strong> returns the summary only in a cluster array.</li>
<li><strong>txt :</strong> returns the summary in a text file and cluster array. (default)</li>
<li><strong>csv : </strong>returns the summary in a comma-separated values (csv) file and cluster array.</li>
</ul>
</li>
</ul></td>
    </tr>
  </tbody>
</table>

<table>
  <tbody>
    <tr>
      <td valign="top" width="70%"><p><img alt="input_array_cluster_1.png" src="assets/input_array_cluster_1.png" width="32"/><strong>init_weight_array : <em>array</em></strong></p>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Integer 32.Png" src="assets/integer-32.png" width="42"/></td>
      <td valign="top"><strong>index : <em>integer</em>,</strong> index of layer.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Enum.Png" src="assets/enum.png" width="42"/></td>
      <td valign="top"><strong>init_weight : <em>enum</em>,</strong> weight initialization mode.</td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img alt="init_weight_array_for_load" src="assets/init_weight_array_for_load.png" width="220"/></p></td>
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

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>
