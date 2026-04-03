<h1>Interleave 1D Array</h1>

<h2>Description</h2>

<p>Interleaves corresponding elements from the input arrays into a single output array.</p>

<p><strong>Warning : A new tensor is created for the output.</strong></p>

<p align="center"><img src="assets/interleave_1d_array.png" alt="Interleave_1D_Array.Png" width="245" /></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Tensor.Png" src="assets/input_tensor.png" width="42"/></td>
      <td valign="top"><strong>arrays : <em>array,</em></strong> array of one-dimentional tensor.</td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Tensor.Png" src="assets/output_tensor.png" width="42"/></td>
      <td valign="top"><strong>interleaved array : <em>class,</em></strong> interleaved array[0] contains array 0[0], interleaved array[1] contains array 1[0], interleaved array[n-1] contains array n-1[0], interleaved array[n] contains array 0[1], and so on, where n is the number of input terminals.</td>
    </tr>
  </tbody>
</table>

<h2>Examples</h2>

<p>All these examples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Accelerator library to run it).</p>

<p align="center"><img src="assets/ex_interleave_1d_array.png" alt="ex_interleave_1d_array" width="260" /></p>
