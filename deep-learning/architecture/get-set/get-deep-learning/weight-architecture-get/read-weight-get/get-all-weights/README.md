<h1>Get all weights</h1>

<h2>Description</h2>

<p>Gets the weights of all layers contained in the model.</p>

<p align="center"><img alt="get_all_weights" src="assets/get_all_weights.PNG" width="220"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Model.Png" src="assets/input_model.png" width="42"/></td>
      <td valign="top"><strong>Model in : </strong>model architecture.</td>
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

<table>
  <tbody>
    <tr>
      <td valign="top" width="70%"><p><img alt="Cluster Array Out.Png" src="assets/cluster-array-out.png" width="32"/><strong>weight_array : <em>array</em></strong></p>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Integer 32 Out.Png" src="assets/integer-32-out.png" width="42"/></td>
      <td valign="top"><strong>index : <em>integer</em>,</strong> index of layer.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="String Out.Png" src="assets/string-out.png" width="42"/></td>
      <td valign="top"><strong>name : <em>string</em>,</strong> name of layer.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="var-out.png" src="assets/var-out.png" width="42"/></td>
      <td valign="top"><strong>weight : <em>variant</em>,</strong> weight value.</td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img alt="out_weight_array" src="assets/out_weight_array.png" width="220"/></p></td>
    </tr>
  </tbody>
</table>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>

<h3>Using the “Get All Weights” function</h3>

<p align="center"><img alt="set_all_random_weights" src="assets/set_all_random_weights.png" width="220"/></p>

<p>1 – Define Graph</p>

<p>We define the graph with one input and two Dense layers named Dense1 and Dense2.</p>

<p>2 – Set Function</p>

<p>We use the “Set All Random Weights” function to create random weights for all layers which have weights in the model.</p>

<p>3 – Get Function</p>

<p>We use the “Get All Weights” function to get the weights of all layers that have them from the model.</p>

<p>4 – Index weight_array</p>

<p>Since the only layers that have weights are Dense1 and Dense2 we index the array returned by the get function to retrieve their weight.</p>

<p>5 – Convert variant to data</p>

<p>The get function returns the weights in a variant, so we use the “Variant To Data” function of LabVIEW to get the result in an array. For that, we use the polymorph which transmits us directly the typedef of the Dense layer.</p>
