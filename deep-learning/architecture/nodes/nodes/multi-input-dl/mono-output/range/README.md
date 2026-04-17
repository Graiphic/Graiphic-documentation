<h1>Range</h1>

<h2>Description</h2>

<p>Generate a tensor containing a sequence of numbers that begin at <code>start</code> and extends by increments of <code>delta</code> up to <code>limit</code> (exclusive).</p>

<p align="center"><img alt="Range" src="assets/Range.png" width="299"/></p>

<p>The number of elements in the output of range is computed as below :</p>

<p>number_of_elements</p>

<p>=</p>

<p>max</p>

<p>(</p>

<p>ceil</p>

<p>(</p>

<p>(</p>

<p>limit</p>

<p>-</p>

<p>start</p>

<p>)</p>

<p>/</p>

<p>delta</p>

<p>)</p>

<p>,</p>

<p>0</p>

<p>)</p>

<p>The pseudocode determining the contents of the output is shown below :</p>

<p>for</p>

<p>(</p>

<p>int</p>

<p>i</p>

<p>=</p>

<p>0</p>

<p>;</p>

<p>i</p>

<p>&lt;</p>

<p>number_of_elements</p>

<p>;</p>

<p>++</p>

<p>i</p>

<p>)</p>

<p>{</p>

<p>output</p>

<p>[</p>

<p>i</p>

<p>]</p>

<p>=</p>

<p>start</p>

<p>+</p>

<p>(</p>

<p>i</p>

<p>*</p>

<p>delta</p>

<p>);</p>

<p>}</p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Array_String.Png" src="assets/input_array_string.png" width="42"/></td>
      <td valign="top"><strong><a href="../../../../../../more-deep-learning/nodes-parameters/specified_outputs_name/README.md">specified_outputs_name</a> : <em>array, </em></strong>this parameter lets you manually assign custom names to the output tensors of a node.</td>
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
      <td valign="top"><strong>Graphs in :</strong> <strong><em>cluster,</em></strong> ONNX model architecture.</td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Object_3.Png" src="assets/input_object_3.png" width="42"/></td>
      <td valign="top"><strong>start (heterogeneous) –</strong> <strong>T :</strong> <em><strong>object,</strong></em> scalar. First entry for the range of output values.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Object_3.Png" src="assets/input_object_3.png" width="42"/></td>
      <td valign="top"><strong>limit (heterogeneous) –</strong> <strong>T :</strong> <em><strong>object,</strong></em> scalar. Exclusive upper limit for the range of output values.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Object_3.Png" src="assets/input_object_3.png" width="42"/></td>
      <td valign="top"><strong>delta (heterogeneous) – T : <em>object, </em></strong>scalar. Value to step by.</td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img alt="input_node_range" src="assets/input_node_range.png" width="220"/></p></td>
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
      <td valign="top"><strong>output (heterogeneous) –</strong> <strong>T : <em>object,</em></strong> a 1-D tensor with same type as the inputs containing generated range of values.</td>
    </tr>
  </tbody>
</table>

<h2>Type Constraints</h2>

<p><strong>T</strong> in (<code>tensor(double)</code>, <code>tensor(float)</code>, <code>tensor(int16)</code>, <code>tensor(int32)</code>, <code>tensor(int64)</code>) : Constrain input types to common numeric type tensors.</p>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>
