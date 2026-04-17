<h1>ScatterND</h1>

<h2>Description</h2>

<p>ScatterND takes three inputs <code>data</code> tensor of rank r &gt;= 1, <code>indices</code> tensor of rank q &gt;= 1, and <code>updates</code> tensor of rank q + r – indices.shape[-1] – 1. The output of the operation is produced by creating a copy of the input <code>data</code>, and then updating its value to values specified by <code>updates</code> at specific index positions specified by <code>indices</code>. Its output shape is the same as the shape of <code>data</code>.</p>

<p align="center"><img alt="ScatterND" src="assets/ScatterND.png" width="299"/></p>

<p><code>indices</code> is an integer tensor. Let k denote indices.shape[-1], the last dimension in the shape of <code>indices</code>. <code>indices</code> is treated as a (q-1)-dimensional tensor of k-tuples, where each k-tuple is a partial-index into <code>data</code>. Hence, k can be a value at most the rank of <code>data</code>. When k equals rank(data), each update entry specifies an update to a single element of the tensor. When k is less than rank(data) each update entry specifies an update to a slice of the tensor. Index values are allowed to be negative, as per the usual convention for counting backwards from the end, but are expected in the valid range.</p>

<p><code>updates</code> is treated as a (q-1)-dimensional tensor of replacement-slice-values. Thus, the first (q-1) dimensions of updates.shape must match the first (q-1) dimensions of indices.shape. The remaining dimensions of <code>updates</code> correspond to the dimensions of the replacement-slice-values. Each replacement-slice-value is a (r-k) dimensional tensor, corresponding to the trailing (r-k) dimensions of <code>data</code>. Thus, the shape of <code>updates</code> must equal indices.shape[0:q-1] ++ data.shape[k:r-1], where ++ denotes the concatenation of shapes.</p>

<p>The <code>output</code> is calculated via the following equation:</p>

<p>output</p>

<p>=</p>

<p>np</p>

<p>.</p>

<p>copy</p>

<p>(</p>

<p>data</p>

<p>)</p>

<p>update_indices</p>

<p>=</p>

<p>indices</p>

<p>.</p>

<p>shape</p>

<p>[:</p>

<p>-</p>

<p>1</p>

<p>]</p>

<p>for</p>

<p>idx</p>

<p>in</p>

<p>np</p>

<p>.</p>

<p>ndindex</p>

<p>(</p>

<p>update_indices</p>

<p>):</p>

<p>output</p>

<p>[</p>

<p>indices</p>

<p>[</p>

<p>idx</p>

<p>]]</p>

<p>=</p>

<p>updates</p>

<p>[</p>

<p>idx</p>

<p>]</p>

<p>The order of iteration in the above loop is not specified. In particular, indices should not have duplicate entries: that is, if idx1 != idx2, then indices[idx1] != indices[idx2]. This ensures that the output value does not depend on the iteration order.</p>

<p><code>reduction</code> allows specification of an optional reduction operation, which is applied to all values in <code>updates</code> tensor into <code>output</code> at the specified <code>indices</code>. In cases where <code>reduction</code> is set to “none”, indices should not have duplicate entries: that is, if idx1 != idx2, then indices[idx1] != indices[idx2]. This ensures that the output value does not depend on the iteration order. When <code>reduction</code> is set to some reduction function <code>f</code>, <code>output</code> is calculated as follows:</p>

<p>output</p>

<p>=</p>

<p>np</p>

<p>.</p>

<p>copy</p>

<p>(</p>

<p>data</p>

<p>)</p>

<p>update_indices</p>

<p>=</p>

<p>indices</p>

<p>.</p>

<p>shape</p>

<p>[:</p>

<p>-</p>

<p>1</p>

<p>]</p>

<p>for</p>

<p>idx</p>

<p>in</p>

<p>np</p>

<p>.</p>

<p>ndindex</p>

<p>(</p>

<p>update_indices</p>

<p>):</p>

<p>output</p>

<p>[</p>

<p>indices</p>

<p>[</p>

<p>idx</p>

<p>]]</p>

<p>=</p>

<p>f</p>

<p>(</p>

<p>output</p>

<p>[</p>

<p>indices</p>

<p>[</p>

<p>idx</p>

<p>]],</p>

<p>updates</p>

<p>[</p>

<p>idx</p>

<p>])</p>

<p>where the <code>f</code> is <code>+</code>, <code>*</code>, <code>max</code> or <code>min</code> as specified.</p>

<p>This operator is the inverse of GatherND.</p>

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
      <td valign="top"><strong>data (heterogeneous) – T : <em>object, </em></strong>tensor of rank r >= 1.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Object_3.Png" src="assets/input_object_3.png" width="42"/></td>
      <td valign="top"><strong>indices (heterogeneous) – tensor(int64) : <em>object, </em></strong>tensor of rank q >= 1.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Object_3.Png" src="assets/input_object_3.png" width="42"/></td>
      <td valign="top"><strong>updates (heterogeneous) – T : <em>object, </em></strong>tensor of rank q + r – indices_shape[-1] – 1.</td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img alt="input_node_scatter_elements" src="assets/input_node_scatter_elements.png" width="220"/></p></td>
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
      <td valign="top"><strong>Parameters : <em>cluster,</em></strong></td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Enum.Png" src="assets/enum.png" width="42"/></td>
      <td valign="top"><strong>reduction : <em>enum,</em></strong> type of reduction to apply: none (default), add, mul, max, min. ‘none’: no reduction applied. ‘add’: reduction using the addition operation. ‘mul’: reduction using the addition operation. ‘max’: reduction using the maximum operation.‘min’: reduction using the minimum operation.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “none”.</td>
    </tr>
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
  </tbody>
</table></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="String.Png" src="assets/string.png" width="42"/></td>
      <td valign="top"><strong>name (optional) :</strong> <em><strong>string,</strong></em> name of the node.</td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img alt="param_node_scatter_nd" src="assets/param_node_scatter_nd.png" width="220"/></p></td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Object_3.Png" src="assets/output_object_3.png" width="42"/></td>
      <td valign="top"><strong>output (heterogeneous) – T : <em>object, </em></strong>tensor of rank r >= 1.</td>
    </tr>
  </tbody>
</table>

<h2>Type Constraints</h2>

<p><strong>T</strong> in (<code>tensor(bfloat16)</code>, <code>tensor(bool)</code>, <code>tensor(complex128)</code>, <code>tensor(complex64)</code>, <code>tensor(double)</code>, <code>tensor(float)</code>, <code>tensor(float16)</code>, <br/><code>tensor(int16)</code>, <code>tensor(int32)</code>, <code>tensor(int64)</code>, <code>tensor(int8)</code>, <code>tensor(string)</code>, <code>tensor(uint16)</code>, <code>tensor(uint32)</code>, <code>tensor(uint64)</code>, <code>tensor(uint8)</code>) : Constrain input and output types to any tensor type.</p>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>
