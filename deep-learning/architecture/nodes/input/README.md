<h1>Input</h1>

<h2>Description</h2>

<p>Setup and add “Input” node into the model during the definition graph step.</p>

<p align="center"><img alt="Input" src="assets/Input.png" width="263"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Integer 32.Png" src="assets/integer-32.png" width="42"/></td>
      <td valign="top"><strong>index : <em>integer, </em></strong>this parameter refers to the position of the input within the ONNX graph. When executing a model with multiple inputs, the index helps you identify which input you are targeting. It is especially useful when configuring input data, using the <strong>Input Data</strong> polymorph found in the <strong>Deep Learning</strong> → <strong>Runtime</strong> palette.</td>
    </tr>
  </tbody>
</table>

<table>
  <tbody>
    <tr>
      <td valign="top" width="70%"><p><img alt="Cluster.Png" src="assets/cluster.png" width="32"/><strong>Parameters : <em>cluster</em></strong></p>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Array Integer 32.Png" src="assets/array-integer-32.png" width="42"/></td>
      <td valign="top"><strong>input_shape : <em>array</em>, </strong>integers defining the shape of the input tensor.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">A negative value indicates that the dimension exists but its size is unknown.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">This array may also be empty if the entire input shape and rank is unknown.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Array_String.Png" src="assets/input_array_string.png" width="42"/></td>
      <td valign="top"><strong>dynamic_shape : <em>array, </em></strong>strings providing symbolic names for each dimension, used when input_shape contains negative values.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Should have the same length as input_shape; if shorter, it will be automatically padded with “unknown” to match the size of input_shape.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Enum.Png" src="assets/enum.png" width="42"/></td>
      <td valign="top"><strong>dtype : <em>enum,</em></strong> the data type for the elements of the output tensor. if not specified, we will use the data type of the input tensor.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “UNDEFINED”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="String.Png" src="assets/string.png" width="42"/></td>
      <td valign="top"><strong>name (optional) :</strong> <em><strong>string,</strong></em> name of the node.</td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img alt="param_node_input" src="assets/param_node_input.png" width="220"/></p></td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Object_3.Png" src="assets/output_object_3.png" width="42"/></td>
      <td valign="top"><strong>Graph out : <em>object, </em></strong>ONNX model architecture.</td>
    </tr>
  </tbody>
</table>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>
