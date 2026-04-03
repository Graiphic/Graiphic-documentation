<h1>Array Size</h1>

<h2>Description</h2>

<p>Returns the number of elements in each dimension of n-dimensional array.</p>

<p align="center"><img src="assets/array_size.png" alt="Array_Size.Png" width="183" /></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Tensor.Png" src="assets/input_tensor.png" width="42"/></td>
      <td valign="top"><strong>array : <em>class, </em></strong>n-dimension tensor.</td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Array_Integer_32.Png" src="assets/output_array_integer_32.png" width="42"/></td>
      <td valign="top"><strong>size(s) : <em>class,</em></strong> returned value is a 1D array in which each element is a 32-bit integer that represents the number of elements in the corresponding dimension of array. The order of elements in the return array corresponds to row-major order. Thus, vol is the first index, followed by page, row, and column. These names are index identifiers and have no other meaning.</td>
    </tr>
  </tbody>
</table>

<h2>Examples</h2>

<p>All these examples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Accelerator library to run it).</p>

<p align="center"><img src="assets/ex_array_size.png" alt="ex_array_size" width="260" /></p>
