<h1>DepthToSpace</h1>

<h2>Description</h2>

<p>DepthToSpace rearranges (permutes) data from depth into blocks of spatial data.</p>

<p align="center"><img alt="DepthToSpace" src="assets/DepthToSpace.png" width="299"/></p>

<p>This is the reverse transformation of SpaceToDepth. More specifically, this op outputs a copy of the input tensor where values from the depth dimension are moved in spatial blocks to the height and width dimensions. By default, <code>mode</code> = <code>DCR</code>. In the DCR mode, elements along the depth dimension from the input tensor are rearranged in the following order: depth, column, and then row. The output y is computed from the input x as below:</p>

<p>b</p>

<p>,</p>

<p>c</p>

<p>,</p>

<p>h</p>

<p>,</p>

<p>w</p>

<p>=</p>

<p>x</p>

<p>.</p>

<p>shape</p>

<p>tmp</p>

<p>=</p>

<p>np</p>

<p>.</p>

<p>reshape</p>

<p>(</p>

<p>x</p>

<p>,</p>

<p>[</p>

<p>b</p>

<p>,</p>

<p>blocksize</p>

<p>,</p>

<p>blocksize</p>

<p>,</p>

<p>c</p>

<p>//</p>

<p>(</p>

<p>blocksize</p>

<p>**</p>

<p>2</p>

<p>),</p>

<p>h</p>

<p>,</p>

<p>w</p>

<p>])</p>

<p>tmp</p>

<p>=</p>

<p>np</p>

<p>.</p>

<p>transpose</p>

<p>(</p>

<p>tmp</p>

<p>,</p>

<p>[</p>

<p>0</p>

<p>,</p>

<p>3</p>

<p>,</p>

<p>4</p>

<p>,</p>

<p>1</p>

<p>,</p>

<p>5</p>

<p>,</p>

<p>2</p>

<p>])</p>

<p>y</p>

<p>=</p>

<p>np</p>

<p>.</p>

<p>reshape</p>

<p>(</p>

<p>tmp</p>

<p>,</p>

<p>[</p>

<p>b</p>

<p>,</p>

<p>c</p>

<p>//</p>

<p>(</p>

<p>blocksize</p>

<p>**</p>

<p>2</p>

<p>),</p>

<p>h</p>

<p>*</p>

<p>blocksize</p>

<p>,</p>

<p>w</p>

<p>*</p>

<p>blocksize</p>

<p>])</p>

<p>In the CRD mode, elements along the depth dimension from the input tensor are rearranged in the following order: column, row, and the depth. The output y is computed from the input x as below :</p>

<p>b, c, h, w = x.shape<br/>
tmp = np.reshape(x, [b, c // (blocksize ** 2), blocksize, blocksize, h, w])<br/>
tmp = np.transpose(tmp, [0, 1, 4, 2, 5, 3])<br/>
y = np.reshape(tmp, [b, c // (blocksize ** 2), h * blocksize, w * blocksize])</p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Array_String.Png" src="assets/input_array_string.png" width="42"/></td>
      <td valign="top"><strong><a href="../../../../../../more-deep-learning/nodes-parameters/specified_outputs_name/README.md">specified_outputs_name</a> : <em>array, </em></strong>this parameter lets you manually assign custom names to the output tensors of a node.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Object_3.Png" src="assets/input_object_3.png" width="42"/></td>
      <td valign="top"><strong>input (heterogeneous) – T : <em>object, </em></strong>input tensor of [N,C,H,W], where N is the batch axis, C is the channel or depth, H is the height and W is the width.</td>
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
      <td width="64" valign="top"><img alt="Integer 32.Png" src="assets/integer-32.png" width="42"/></td>
      <td valign="top"><strong>blocksize : <em>integer, </em></strong>blocks of [blocksize, blocksize] are moved.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “0”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Enum.Png" src="assets/enum.png" width="42"/></td>
      <td valign="top"><strong>mode : <em>enum, </em></strong>DCR for depth-column-row order re-arrangement. Use CRD for column-row-depth order.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “DCR”.</td>
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
    <tr>
      <td width="64" valign="top"><img alt="String.Png" src="assets/string.png" width="42"/></td>
      <td valign="top"><strong>name (optional) :</strong> <em><strong>string,</strong></em> name of the node.</td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img alt="param_node_depth_to_space" src="assets/param_node_depth_to_space.png" width="220"/></p></td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Object_3.Png" src="assets/output_object_3.png" width="42"/></td>
      <td valign="top"><strong>output (heterogeneous) – T : <em>object, </em></strong>output tensor of [N, C/(blocksize * blocksize), H * blocksize, W * blocksize].</td>
    </tr>
  </tbody>
</table>

<h2>Type Constraints</h2>

<p><strong>T</strong> in (<code>tensor(bfloat16)</code>, <code>tensor(bool)</code>, <code>tensor(complex128)</code>, <code>tensor(complex64)</code>, <code>tensor(double)</code>, <code>tensor(float)</code>, <code>tensor(float16)</code>,<br/><code>tensor(int16)</code>, <code>tensor(int32)</code>, <code>tensor(int64)</code>, <code>tensor(int8)</code>, <code>tensor(string)</code>, <code>tensor(uint16)</code>, <code>tensor(uint32)</code>, <code>tensor(uint64)</code>, <code>tensor(uint8)</code>) : Constrain input and output types to all tensor types.</p>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>
