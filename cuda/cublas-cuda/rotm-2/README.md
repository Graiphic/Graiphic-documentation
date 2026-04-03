<h1>rotm</h1>

<h2>Description</h2>

<p>This function applies the modified Givens transformation to vectors x and y. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img src="assets/rotm.png" alt="Rotm.Png" width="209" /></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Tensor.Png" src="assets/input_tensor.png" width="42"/></td>
      <td valign="top"><strong>x : <em>class, </em></strong>tensor of a vector with n elements.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Tensor.Png" src="assets/input_tensor.png" width="42"/></td>
      <td valign="top"><strong>y : <em>class, </em></strong>tensor of a vector with n elements.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Interger_32.Png" src="assets/input_interger_32.png" width="42"/></td>
      <td valign="top"><strong>incx : <em>integer,</em></strong> stride between consecutive elements of x.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Interger_32.Png" src="assets/input_interger_32.png" width="42"/></td>
      <td valign="top"><strong>incy : <em>integer,</em></strong> stride between consecutive elements of y.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Array_Single.Png" src="assets/input_array_single.png" width="42"/></td>
      <td valign="top"><strong>param : <em>array,</em></strong> vector of 5 elements, where param[0] and param[1-4] contain the flag and matrix <em>H</em>.</td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Tensor.Png" src="assets/output_tensor.png" width="42"/></td>
      <td valign="top"><strong>x : <em>class, </em></strong>tensor of a vector with n elements.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Tensor.Png" src="assets/output_tensor.png" width="42"/></td>
      <td valign="top"><strong>y : <em>class, </em></strong>tensor of a vector with n elements.</td>
    </tr>
  </tbody>
</table>

<h2>Examples</h2>

<p>All these examples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Accelerator library to run it).</p>

<p align="center"><img src="assets/ex_rotm.png" alt="ex_rotm" width="260" /></p>
