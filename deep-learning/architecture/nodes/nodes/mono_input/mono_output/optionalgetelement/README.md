<h1>OptionalGetElement</h1>

<h2>Description</h2>

<p>If the input is a tensor or sequence type, it returns the input. If the input is an optional type, it outputs the element in the input. It is an error if the input is an empty optional-type (i.e. does not have an element) and the behavior is undefined in this case.</p>

<p align="center"><img alt="node_optional_get_element.png" src="assets/node_optional_get_element.png" width="299"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Array_String.Png" src="assets/input_array_string.png" width="42"/></td>
      <td valign="top"><strong><a href="../../../../../../more-deep-learning/nodes-parameters/specified_outputs_name/README.md">specified_outputs_name</a> : <em>array, </em></strong>this parameter lets you manually assign custom names to the output tensors of a node.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Object_3.Png" src="assets/input_object_3.png" width="42"/></td>
      <td valign="top"><strong>input (optional, heterogeneous) – O : <em>object, </em></strong>the optional input.</td>
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
      <td valign="top"><strong>name (optional) :</strong> <em><strong>string,</strong></em> name of the node.</td>
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
      <td width="64" valign="top"><img alt="Output_Object_3.Png" src="assets/output_object_3.png" width="42"/></td>
      <td valign="top"><strong>output (heterogeneous) – V : <em>object, </em></strong>output element in the optional input.</td>
    </tr>
  </tbody>
</table>

<h2>Type Constraints</h2>

<p><strong>O</strong> in (<code>optional(seq(tensor(bool)))</code>, <code>optional(seq(tensor(complex128)))</code>, <code>optional(seq(tensor(complex64)))</code>,<br/><code>optional(seq(tensor(double)))</code>, <code>optional(seq(tensor(float)))</code>, <code>optional(seq(tensor(float16)))</code>, <code>optional(seq(tensor(int16)))</code>, <code>optional(seq(tensor(int32)))</code>, <code>optional(seq(tensor(int64)))</code>, <code>optional(seq(tensor(int8)))</code>, <code>optional(seq(tensor(string)))</code>, <code>optional(seq(tensor(uint16)))</code>, <code>optional(seq(tensor(uint32)))</code>, <code>optional(seq(tensor(uint64)))</code>, <code>optional(seq(tensor(uint8)))</code>, <code>optional(tensor(bool))</code>, <code>optional(tensor(complex128))</code>, <code>optional(tensor(complex64))</code>, <code>optional(tensor(double))</code>, <code>optional(tensor(float))</code>, <code>optional(tensor(float16))</code>, <code>optional(tensor(int16))</code>, <code>optional(tensor(int32))</code>, <code>optional(tensor(int64))</code>, <code>optional(tensor(int8))</code>, <code>optional(tensor(string))</code>, <code>optional(tensor(uint16))</code>, <code>optional(tensor(uint32))</code>, <code>optional(tensor(uint64))</code>, <code>optional(tensor(uint8))</code>, <code>seq(tensor(bool))</code>, <code>seq(tensor(complex128))</code>, <code>seq(tensor(complex64))</code>, <code>seq(tensor(double))</code>, <code>seq(tensor(float))</code>, <code>seq(tensor(float16))</code>, <code>seq(tensor(int16))</code>, <code>seq(tensor(int32))</code>, <code>seq(tensor(int64))</code>, <code>seq(tensor(int8))</code>, <code>seq(tensor(string))</code>, <code>seq(tensor(uint16))</code>, <code>seq(tensor(uint32))</code>, <code>seq(tensor(uint64))</code>, <code>seq(tensor(uint8))</code>, <code>tensor(bool)</code>, <code>tensor(complex128)</code>, <code>tensor(complex64)</code>, <code>tensor(double)</code>, <code>tensor(float)</code>, <code>tensor(float16)</code>, <code>tensor(int16)</code>, <code>tensor(int32)</code>, <code>tensor(int64)</code>, <code>tensor(int8)</code>, <code>tensor(string)</code>, <code>tensor(uint16)</code>, <code>tensor(uint32)</code>, <code>tensor(uint64)</code>, <code>tensor(uint8)</code>) : Constrain input type to optional tensor and optional sequence types.</p>

<p><strong>V</strong> in (<code>seq(tensor(bool))</code>, <code>seq(tensor(complex128))</code>, <code>seq(tensor(complex64))</code>, <code>seq(tensor(double))</code>, <code>seq(tensor(float))</code>,<br/>
<code>seq(tensor(float16))</code>, <code>seq(tensor(int16))</code>, <code>seq(tensor(int32))</code>, <code>seq(tensor(int64))</code>, <code>seq(tensor(int8))</code>, <code>seq(tensor(string))</code>, <code>seq(tensor(uint16))</code>, <code>seq(tensor(uint32))</code>, <code>seq(tensor(uint64))</code>, <code>seq(tensor(uint8))</code>, <code>tensor(bool)</code>, <code>tensor(complex128)</code>, <code>tensor(complex64)</code>, <code>tensor(double)</code>, <code>tensor(float)</code>, <code>tensor(float16)</code>, <code>tensor(int16)</code>, <code>tensor(int32)</code>, <code>tensor(int64)</code>, <code>tensor(int8)</code>, <code>tensor(string)</code>, <code>tensor(uint16)</code>, <code>tensor(uint32)</code>, <code>tensor(uint64)</code>, <code>tensor(uint8)</code>) : Constrain output type to all tensor or sequence types.</p>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>
