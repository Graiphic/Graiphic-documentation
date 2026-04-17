<h1>MicrosoftUnique</h1>

<h2>Description</h2>

<p>Finds all the unique values (deduped list) present in the given input tensor. This operator returns 3 outputs. The first output tensor ‘uniques’ contains all of the unique elements of the input, sorted in the same order that they occur in the input. The second output tensor ‘idx’ is the same size as the input and it contains the index of each value of the input in ‘uniques’. The third output tensor ‘counts’ contains the count of each element of ‘uniques’ in the input. Example: input_x = [2, 1, 1, 3, 4, 3] output_uniques = [2, 1, 3, 4] output_idx = [0, 1, 1, 2, 3, 2] output_counts = [1, 2, 2, 1].</p>

<p align="center"><img alt="MicrosoftUnique" src="assets/MicrosoftUnique.png" width="311"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Array_String.Png" src="assets/input_array_string.png" width="42"/></td>
      <td valign="top"><strong><a href="../../../../../../more-deep-learning/nodes-parameters/specified_outputs_name/README.md">specified_outputs_name</a> : <em>array, </em></strong>this parameter lets you manually assign custom names to the output tensors of a node.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Object_3.Png" src="assets/input_object_3.png" width="42"/></td>
      <td valign="top"><strong>x (heterogeneous) – T : <em>object, </em></strong>a 1-D input tensor that is to be processed.</td>
    </tr>
  </tbody>
</table>

<table>
  <tbody>
    <tr>
      <td valign="top" width="70%"><p><img alt="Cluster.Png" src="assets/cluster.png" width="32"/><strong>Parameters : <em>cluster,</em></strong></p>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Booleen.Png" src="assets/booleen.png" width="42"/></td>
      <td valign="top"><strong>training? :</strong> <em><strong>boolean</strong></em>, whether the layer is in training mode (can store data for backward).</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “True”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Double.Png" src="assets/double.png" width="42"/></td>
      <td valign="top"><strong>lda coeff :</strong> <em><strong>float</strong></em>, defines the coefficient by which the loss derivative will be multiplied before being sent to the previous layer (since during the backward run we go backwards).</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “1”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="String.Png" src="assets/string.png" width="42"/></td>
      <td valign="top"><strong>name (optional) :</strong> <em><strong>string,</strong></em> name of the node.</td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img src="assets/layer_param.png" alt="layer_param" width="220" /></p></td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td valign="top" width="70%"><p><img alt="Cluster Out.Png" src="assets/cluster-out.png" width="32"/><strong>Graphs out :</strong><strong><em>cluster,</em></strong> ONNX model architecture.</p>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Object_3.Png" src="assets/output_object_3.png" width="42"/></td>
      <td valign="top"><strong>y (heterogeneous) – T : <em>object, </em></strong>a 1-D tensor of the same type as ‘x’ containing all the unique values in ‘x’ sorted in the same order that they occur in the input ‘x’</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Object_3.Png" src="assets/output_object_3.png" width="42"/></td>
      <td valign="top"><strong>idx (heterogeneous) – tensor(int64) : <em>object, </em></strong>a 1-D INT64 tensor of the same size as ‘x’ containing the indices for each value in ‘x’ in the output ‘uniques’.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Object_3.Png" src="assets/output_object_3.png" width="42"/></td>
      <td valign="top"><strong>counts (heterogeneous) – tensor(int64) : <em>object, </em></strong>a 1-D INT64 tensor containing the the count of each element of ‘uniques’ in the input ‘x’.</td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img alt="output_node_microsoft_unique" src="assets/output_node_microsoft_unique.png" width="220"/></p></td>
    </tr>
  </tbody>
</table>

<h2>Type Constraints</h2>

<p><strong>T</strong> in (<code>tensor(uint8)</code>, <code>tensor(uint16)</code>, <code>tensor(uint32)</code>, <code>tensor(uint64)</code>, <code>tensor(int8)</code>, <code>tensor(int16)</code>, <code>tensor(int32)</code>,<br/><code>tensor(int64)</code>, <code>tensor(float16)</code>, <code>tensor(float)</code>, <code>tensor(double)</code>, <code>tensor(string)</code>, <code>tensor(bool)</code>, <code>tensor(complex64)</code>, <code>tensor(complex128)</code>) : Input can be of any tensor type.</p>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>
