<h1>LpPool</h1>

<h2>Description</h2>

<p>Lp pooling consisting of computing the Lp norm on all values of a subset of the input tensor according to the kernel size and downsampling the data into the output tensor Y for further processing.</p>

<p align="center"><img alt="LpPool" src="assets/LpPool.png" width="299"/></p>

<p>LpPool consumes an input tensor X and applies Lp pooling across the tensor according to kernel sizes, stride sizes, and pad lengths. The output spatial shape will be following :</p>

<p>output_spatial_shape</p>

<p>[</p>

<p>i</p>

<p>]</p>

<p>=</p>

<p>floor</p>

<p>((</p>

<p>input_spatial_shape</p>

<p>[</p>

<p>i</p>

<p>]</p>

<p>+</p>

<p>pad_shape</p>

<p>[</p>

<p>i</p>

<p>]</p>

<p>-</p>

<p>{</p>

<p>kernelSpatialShape</p>

<p>})</p>

<p>/</p>

<p>strides_spatial_shape</p>

<p>[</p>

<p>i</p>

<p>]</p>

<p>+</p>

<p>1</p>

<p>)</p>

<p>or</p>

<p>output_spatial_shape</p>

<p>[</p>

<p>i</p>

<p>]</p>

<p>=</p>

<p>ceil</p>

<p>((</p>

<p>input_spatial_shape</p>

<p>[</p>

<p>i</p>

<p>]</p>

<p>+</p>

<p>pad_shape</p>

<p>[</p>

<p>i</p>

<p>]</p>

<p>-</p>

<p>{</p>

<p>kernelSpatialShape</p>

<p>})</p>

<p>/</p>

<p>strides_spatial_shape</p>

<p>[</p>

<p>i</p>

<p>]</p>

<p>+</p>

<p>1</p>

<p>)</p>

<p>if ceil_mode is enabled <code>pad_shape</code> is the sum of pads along axis <code>i</code>.</p>

<p><code>auto_pad</code> is a DEPRECATED attribute. If you are using them currently, the output spatial shape will be following:</p>

<p>VALID</p>

<p>:</p>

<p>output_spatial_shape</p>

<p>[</p>

<p>i</p>

<p>]</p>

<p>=</p>

<p>ceil</p>

<p>((</p>

<p>input_spatial_shape</p>

<p>[</p>

<p>i</p>

<p>]</p>

<p>-</p>

<p>{</p>

<p>kernelSpatialShape</p>

<p>}</p>

<p>+</p>

<p>1</p>

<p>)</p>

<p>/</p>

<p>strides_spatial_shape</p>

<p>[</p>

<p>i</p>

<p>])</p>

<p>SAME_UPPER</p>

<p>or</p>

<p>SAME_LOWER</p>

<p>:</p>

<p>output_spatial_shape</p>

<p>[</p>

<p>i</p>

<p>]</p>

<p>=</p>

<p>ceil</p>

<p>(</p>

<p>input_spatial_shape</p>

<p>[</p>

<p>i</p>

<p>]</p>

<p>/</p>

<p>strides_spatial_shape</p>

<p>[</p>

<p>i</p>

<p>])</p>

<p>And pad shape will be following if <code>SAME_UPPER</code> or <code>SAME_LOWER</code>:</p>

<p>pad_shape</p>

<p>[</p>

<p>i</p>

<p>]</p>

<p>=</p>

<p>(</p>

<p>output_spatial_shape</p>

<p>[</p>

<p>i</p>

<p>]</p>

<p>-</p>

<p>1</p>

<p>)</p>

<p>*</p>

<p>strides_spatial_shape</p>

<p>[</p>

<p>i</p>

<p>]</p>

<p>+</p>

<p>{</p>

<p>kernelSpatialShape</p>

<p>}</p>

<p>-</p>

<p>input_spat</p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Array_String.Png" src="assets/input_array_string.png" width="42"/></td>
      <td valign="top"><strong><a href="../../../../../../more-deep-learning/nodes-parameters/specified_outputs_name/README.md">specified_outputs_name</a> : <em>array, </em></strong>this parameter lets you manually assign custom names to the output tensors of a node.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Object_3.Png" src="assets/input_object_3.png" width="42"/></td>
      <td valign="top"><strong>X (heterogeneous) – T : <em>object, </em></strong>input data tensor from the previous operator; dimensions for image case are (N x C x H x W), where N is the batch size, C is the number of channels, and H and W are the height and the width of the data. For non image case, the dimensions are in the form of (N x C x D1 x D2 … Dn), where N is the batch size.</td>
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
      <td width="64" valign="top"><img alt="Enum.Png" src="assets/enum.png" width="42"/></td>
      <td valign="top"><strong>auto_pad : <em>enum,</em></strong> auto_pad must be either NOTSET, SAME_UPPER, SAME_LOWER or VALID. Where default value is NOTSET, which means explicit padding is used. SAME_UPPER or SAME_LOWER mean pad the input so that <code>output_shape = ceil(input_shape / strides)</code> for each axis <code>i</code>. The padding is split between the two sides equally or almost equally (depending on whether it is even or odd). In case the padding is an odd number, the extra padding is added at the end for SAME_UPPER and at the beginning for SAME_LOWER.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “NOTSET”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Booleen.Png" src="assets/booleen.png" width="42"/></td>
      <td valign="top"><strong>ceil_mode</strong> <strong>:</strong> <em><strong>boolean</strong></em>, whether to use ceil or floor (default) to compute the output shape.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “False”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Array_Integer_64.Png" src="assets/input_array_integer_64.png" width="42"/></td>
      <td valign="top"><strong>dilations : <em>array,</em></strong> dilation value along each spatial axis of the filter. If not present, the dilation defaults is 1 along each spatial axis.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “empty”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Array_Integer_64.Png" src="assets/input_array_integer_64.png" width="42"/></td>
      <td valign="top"><strong>kernel_shape : <em>array,</em></strong> the size of the kernel along each axis.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “empty”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Integer 32.Png" src="assets/integer-32.png" width="42"/></td>
      <td valign="top"><strong>p : <em>integer,</em></strong> p value of the Lp norm used to pool over the input data.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “2”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Array_Integer_64.Png" src="assets/input_array_integer_64.png" width="42"/></td>
      <td valign="top"><strong>pads</strong> <strong>: <em>array,</em></strong> padding for the beginning and ending along each spatial axis, it can take any value greater than or equal to 0. The value represent the number of pixels added to the beginning and end part of the corresponding axis. <code>pads</code> format should be as follow [x1_begin, x2_begin…x1_end, x2_end,…], where xi_begin the number of pixels added at the beginning of axis <code>i</code> and xi_end, the number of pixels added at the end of axis <code>i</code>. This attribute cannot be used simultaneously with auto_pad attribute. If not present, the padding defaults to 0 along start and end of each spatial axis.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “empty”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Array_Integer_64.Png" src="assets/input_array_integer_64.png" width="42"/></td>
      <td valign="top"><strong>strides : <em>array,</em></strong> stride along each spatial axis. If not present, the stride defaults to 1 along each spatial axis.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “empty”.</td>
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
      <td valign="top" width="30%"><p align="center"><img alt="param_node_lp_pool" src="assets/param_node_lp_pool.png" width="220"/></p></td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Object_3.Png" src="assets/output_object_3.png" width="42"/></td>
      <td valign="top"><strong>Y (heterogeneous) – T : <em>object, </em></strong>output data tensor from Lp pooling across the input tensor. Dimensions will vary based on various kernel, stride, and pad sizes.</td>
    </tr>
  </tbody>
</table>

<h2>Type Constraints</h2>

<p><strong>T</strong> in (<code>tensor(double)</code>, <code>tensor(float)</code>, <code>tensor(float16)</code>) : Constrain input and output types to float tensors.</p>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>
