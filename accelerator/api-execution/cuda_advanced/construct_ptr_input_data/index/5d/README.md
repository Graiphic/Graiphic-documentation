<h1>5D</h1>

<h2>Description</h2>

<p>Adds to the ptr input array a 5D array (of type <strong>BOOL</strong>, <strong>SGL</strong>, <strong>INT</strong>, <strong>UINT</strong>, or <strong>STRING</strong>) at a specified index. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img src="assets/acc_execution_cuda-advanced_construct-ptr_index_5d.png" alt="Acc_Execution_Cuda Advanced_Construct Ptr_Index_5D.Png" width="243" /></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Array Single.Png" src="assets/array-single.png" width="42"/></td>
      <td valign="top"><strong>5D Input Data : <em>array</em>, </strong>5D array of data with any type : integers (signed/unsigned), floats, doubles, booleans, or strings.</td>
    </tr>
  </tbody>
</table>

<table>
  <tbody>
    <tr>
      <td valign="top" width="70%"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Cluster Array In.Png" src="assets/cluster-array-in.png" width="42"/></td>
      <td valign="top"><strong>Data in : <em>array,</em></strong></td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Unsigned_32.Png" src="assets/input_unsigned_32.png" width="42"/></td>
      <td valign="top"><strong>input_order : <em>integer</em>,</strong> defines the position of the output within the data array. It corresponds to the index assigned to the output when it is created (via the index parameter).</td>
    </tr>
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
</table></td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img src="assets/acc_execution_cuda-advanced_multi_preallocated_input_parameter.png" alt="acc_execution_cuda-advanced_multi_preallocated_input_parameter" width="231" /></p></td>
    </tr>
  </tbody>
</table>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Integer 32.Png" src="assets/integer-32.png" width="42"/></td>
      <td valign="top"><strong>input order : <em>integer</em>,</strong> defines the position of the input within the data array. It corresponds to the index assigned to the input when it is created (via the <i>index</i> parameter).</td>
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
      <td valign="top"><strong>Data in : <em>array,</em></strong></td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Unsigned_32.Png" src="assets/output_unsigned_32.png" width="42"/></td>
      <td valign="top"><strong>input_order : <em>integer</em>,</strong> defines the position of the output within the data array. It corresponds to the index assigned to the output when it is created (via the index parameter).</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Cluster Out.Png" src="assets/cluster-out.png" width="42"/></td>
      <td valign="top"><strong>Inputs Info : <em>cluster</em></strong></td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Unsigned_64.Png" src="assets/output_unsigned_64.png" width="42"/></td>
      <td valign="top"><strong>inputs_ptr : <em>integer, </em></strong>represents a pre-allocated device memory address (for example, a CUDA device pointer) where the input tensor data is already stored.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Array_Integer_64.Png" src="assets/output_array_integer_64.png" width="42"/></td>
      <td valign="top">inputs_shapes :<em> array, </em>specifies the shape of the output tensor. Since the data is written into a pre-allocated device buffer, this shape allows the runtime to interpret the memory layout correctly.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Interger_64.Png" src="assets/output_interger_64.png" width="42"/></td>
      <td valign="top">inputs_ranks :<em> integer, </em>indicates the rank of the tensor, i.e. the number of dimensions (Scalar = 0, 1D = 1, 2D = 2, etc.).</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Enum.Png" src="assets/output_enum.png" width="42"/></td>
      <td valign="top">inputs_types :<em> enum, </em>defines the ONNX tensor type as an enumerated value (e.g. FLOAT, INT64, STRING).</td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img src="assets/acc_execution_cuda-advanced_multi_preallocated_input_parameter.png" alt="acc_execution_cuda-advanced_multi_preallocated_input_parameter" width="231" /></p></td>
    </tr>
  </tbody>
</table>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Accelerator library to run it).</p>
