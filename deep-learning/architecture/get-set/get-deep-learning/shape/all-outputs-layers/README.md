<h1>All outputs layers shape</h1>

<h2>Description</h2>

<p>Gets the output form of the model.</p>

<p align="center"><img alt="get_all_input_shape" src="assets/get_all_input_shape.PNG" width="220"/></p>

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
      <td valign="top" width="70%"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Cluster Array Out.Png" src="assets/cluster-array-out.png" width="42"/></td>
      <td valign="top"><strong>output_array : <em>array,</em></strong></td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Cluster Out.Png" src="assets/cluster-out.png" width="42"/></td>
      <td valign="top"><strong>Name : <em>cluster,</em></strong></td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="String Out.Png" src="assets/string-out.png" width="42"/></td>
      <td valign="top"><strong>node : <em>string</em>,</strong> name of the ONNX node producing the output (e.g., <code>Dense_342_output</code>).</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="String Out.Png" src="assets/string-out.png" width="42"/></td>
      <td valign="top"><strong>output : <em>string</em>,</strong> identifier of the output tensor from this node.</td>
    </tr>
  </tbody>
</table></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Integer 32 Out.Png" src="assets/integer-32-out.png" width="42"/></td>
      <td valign="top"><strong>index : <em>integer</em>,</strong> index of the node within the ONNX graph, used to perform <code>get</code> or <code>set</code> operations on a specific node.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Integer 32 Out.Png" src="assets/integer-32-out.png" width="42"/></td>
      <td valign="top"><strong>output_order : <em>integer</em>,</strong> index of the output (useful to retrieve the data after execution if there are multiple outputs).</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Out Array Integer 32.Png" src="assets/out-array-integer-32.png" width="42"/></td>
      <td valign="top"><strong>output_shape : <em>array</em>,</strong> expected shape of the output tensor. This shape is only valid for models using explicit <code>Layers</code>, and the first dimension always corresponds to the batch size (even if shown as 1 here).</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="output_enum.png" src="assets/output_enum.png" width="42"/></td>
      <td valign="top"><strong>dtype : <em>enum, </em></strong>data type of the output tensor (e.g., <code>FLOAT</code> for floating-point tensors).</td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img alt="output_shape_array" src="assets/output_shape_array.png" width="220"/></p></td>
    </tr>
  </tbody>
</table>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>

<h3>Using the “Get All Output Layer Shape” function</h3>

<p align="center"><img alt="get_all_output_layer_shape" src="assets/get_all_output_layer_shape.png" width="220"/></p>

<p>1 – Define Graph</p>

<p>We define two graphs with two dense layers each and an input of different size.</p>

<p>2 – Merge Function</p>

<p>We use the “Merge” function to merge the two graphs.</p>

<p>3 – Get Function</p>

<p>We use the function “Get All Output Layer Shape” to get the output(s) form of the model.</p>
