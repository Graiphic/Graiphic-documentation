<h1>Rotate 1D Array</h1>

<h2>Description</h2>

<p>Rotates the elements of array the number of places and in the direction indicated by n.</p>

<p align="center"><img src="assets/rotate_1d_array.png" alt="Rotate_1D_Array.Png" width="213" /></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Tensor.Png" src="assets/input_tensor.png" width="42"/></td>
      <td valign="top"><strong>array : <em>class,</em></strong> one-dimentional tensor.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Interger_32.Png" src="assets/input_interger_32.png" width="42"/></td>
      <td valign="top"><strong>n : <em>integer,</em></strong> must be a numeric data type. The function coerces n to a 32-bit integer if you wire another representation to it.</td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Tensor.Png" src="assets/output_tensor.png" width="42"/></td>
      <td valign="top"><strong>rotate array : <em>class,</em></strong> is the output array. For example, if n is 1, the input array[0] becomes output array[1], input array[1] becomes output array[2], and so on, and input array[m–1] becomes output array[0], where m is the number of elements in the array. If n is –2, input array[0] becomes output array[m–2], input array[1] becomes output array[m–1], and so on, and input array[m–1] becomes output array[m–3], where m is the number of elements in the array.</td>
    </tr>
  </tbody>
</table>

<h2>Examples</h2>

<p>All these examples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Accelerator library to run it).</p>

<p align="center"><img src="assets/ex_rotate_1d_array.png" alt="ex_rotate_1d_array" width="260" /></p>
