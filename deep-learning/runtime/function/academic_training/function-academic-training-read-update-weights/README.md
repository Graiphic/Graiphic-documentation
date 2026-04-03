<h1>Read and Update Weights</h1>

<h2>Description</h2>

<p>Read all model weights (trainable and frozen) from the Academic Training Session and update the Inference Session weights.</p>

<p align="center"><img src="assets/function_academic_read_update_weights.png" alt="function_academic_read_update_weights" width="260" /></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Academic.Png" src="assets/input_academic.png" width="42"/></td>
      <td valign="top"><strong>Academic Training in</strong> <strong>: <em>object, </em></strong>academic training session.</td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Academic.Png" src="assets/output_academic.png" width="42"/></td>
      <td valign="top"><strong>Academic Training out</strong> <strong>: <em>object, </em></strong>academic training session.</td>
    </tr>
  </tbody>
</table>

<table>
  <tbody>
    <tr>
      <td valign="top" width="70%"><p align="center"><img src="assets/cluster-out.png" alt="Cluster Out.Png" width="32" /></p>

<p>Weights Info</p>

<p><strong>: <em>cluster</em></strong></p>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="String_Array_Out.Png" src="assets/string_array_out.png" width="42"/></td>
      <td valign="top"><strong> weight_names</strong> <strong>: <em>array,</em></strong> list of names identifying each weight tensor used for training or marked as frozen. These correspond to a subset of the model’s initializers, specifically those involved in learning or fixed parameters, not all initializers present in the ONNX graph.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Array_Unsigned_8.Png" src="assets/output_array_unsigned_8.png" width="42"/></td>
      <td valign="top"><strong> raw_data_out : <em>array,</em></strong> raw byte representation of each weight tensor, flattened into 1D. This field stores the actual binary content of the tensor.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Array_Integer_64.Png" src="assets/output_array_integer_64.png" width="42"/></td>
      <td valign="top"><strong> data_shapes</strong> <strong>: <em>array,</em></strong> shape of each tensor, provided as an array of dimensions. This allows reconstructing the original structure of the tensor from the flattened <code>raw_data_out</code>.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Out Array Integer 32.Png" src="assets/out-array-integer-32.png" width="42"/></td>
      <td valign="top"><strong> data_types</strong> <strong>: <em>array,</em></strong> ONNX data type (enum) of each tensor, such as <code>FLOAT</code>, <code>INT32</code>, <code>FLOAT16</code>, etc. Defines how to interpret the raw bytes.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Array_Integer_64.Png" src="assets/output_array_integer_64.png" width="42"/></td>
      <td valign="top"><strong> data_ranks</strong> <strong>: <em>array,</em></strong> rank of each tensor (number of dimensions), for example :
<ul>
<li>
<ul>
<li>
<ul>
<li>
<ul>
<li>Scalar → 0</li>
<li>Vector → 1</li>
<li>Matrix → 2</li>
<li>Higher-order tensors → 3+</li>
</ul>
</li>
</ul>
</li>
</ul>
</li>
</ul></td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img src="assets/function_training_weights_parameters.png" alt="function_training_weights_parameters" width="153" /></p></td>
    </tr>
  </tbody>
</table>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>
