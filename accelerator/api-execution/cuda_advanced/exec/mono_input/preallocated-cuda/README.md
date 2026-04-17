<h1>Preallocated CUDA</h1>

<h2>Description</h2>

<p>Execute the model using CUDA mono input and mono output pointer. Type : <em><strong>polymorphic</strong><strong>.<br/></strong></em><strong>Warning : This function can only be executed with CUDA or TensorRT.<br/>Both input and output buffer must be pre-allocated on the GPU and managed by the user (no automatic allocation or release).</strong></p>

<p align="center"><img alt="Preallocated CUDA" src="assets/Preallocated CUDA.png" width="263"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Acc_Inference.Png" src="assets/input_acc_inference.png" width="42"/></td>
      <td valign="top"><strong>Inference in</strong> <strong>: <em>object, </em></strong>inference session.</td>
    </tr>
  </tbody>
</table>

<table>
  <tbody>
    <tr>
      <td valign="top" width="70%"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Cluster.Png" src="assets/cluster.png" width="42"/></td>
      <td valign="top"><strong>Inputs Info : <em>cluster</em></strong></td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Unsigned_64.Png" src="assets/input_unsigned_64.png" width="42"/></td>
      <td valign="top"><strong>inputs_ptr : <em>integer, </em></strong>represents a pre-allocated device memory address (for example, a CUDA device pointer) where the input tensor data is already stored.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Array_Integer_64.Png" src="assets/input_array_integer_64.png" width="42"/></td>
      <td valign="top">inputs_shapes :<em> array, </em>specifies the shape of the output tensor. Since the data is written into a pre-allocated device buffer, this shape allows the runtime to interpret the memory layout correctly.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Interger_64.Png" src="assets/input_interger_64.png" width="42"/></td>
      <td valign="top">inputs_ranks :<em> integer, </em>indicates the rank of the tensor, i.e. the number of dimensions (Scalar = 0, 1D = 1, 2D = 2, etc.).</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Enum.Png" src="assets/enum.png" width="42"/></td>
      <td valign="top">inputs_types :<em> enum, </em>defines the ONNX tensor type as an enumerated value (e.g. FLOAT, INT64, STRING).</td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table>

<p>​</p></td>
      <td valign="top" width="30%"><p align="center"><img src="assets/acc_execution_cuda-advanced_mono_preallocated_input_parameter.png" alt="acc_execution_cuda-advanced_mono_preallocated_input_parameter" width="153" /></p></td>
    </tr>
  </tbody>
</table>

<table>
  <tbody>
    <tr>
      <td valign="top" width="70%"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Cluster.Png" src="assets/cluster.png" width="42"/></td>
      <td valign="top"><strong>Outputs Info : <em>cluster</em></strong></td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Unsigned_64.Png" src="assets/input_unsigned_64.png" width="42"/></td>
      <td valign="top"><strong>outputs_ptr : <em>integer, </em></strong>contains the raw byte representation of the input tensor data, stored as a 1D flattened buffer.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Array_Integer_64.Png" src="assets/input_array_integer_64.png" width="42"/></td>
      <td valign="top">outputs_shapes :<em> array, </em>specifies the shape of the output tensor. Since the data is written into a pre-allocated device buffer, this shape allows the runtime to interpret the memory layout correctly.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Interger_64.Png" src="assets/input_interger_64.png" width="42"/></td>
      <td valign="top">outputs_ranks :<em> integer, </em>indicates the rank of the tensor, i.e. the number of dimensions (Scalar = 0, 1D = 1, 2D = 2, etc.).</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Enum.Png" src="assets/enum.png" width="42"/></td>
      <td valign="top">outputs_types :<em> enum, </em>defines the ONNX tensor type as an enumerated value (e.g. FLOAT, INT64, STRING).</td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table>

<p>​</p></td>
      <td valign="top" width="30%"><p align="center"><img src="assets/acc_execution_cuda-advanced_mono_preallocated_output_parameter.png" alt="acc_execution_cuda-advanced_mono_preallocated_output_parameter" width="153" /></p></td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Acc_Inference.Png" src="assets/output_acc_inference.png" width="42"/></td>
      <td valign="top"><strong>Inference out</strong> <strong>: <em>object, </em></strong>inference session.</td>
    </tr>
  </tbody>
</table>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Accelerator library to run it).</p>
