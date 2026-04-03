<h1>Min & Max</h1>

<h2>Description</h2>

<p>Returns the maximum and minimum values found in array, along with the indexes for each value. Type : <em><strong>Polyporphic.</strong></em> </p>

<p align="center"><img src="assets/min_and_max.png" alt="Min_And_Max.Png" width="225" /></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Tensor.Png" src="assets/input_tensor.png" width="42"/></td>
      <td valign="top"><strong>array : <em>class,</em></strong> n-dimensional tensor.</td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Single.Png" src="assets/output_single.png" width="42"/></td>
      <td valign="top"><strong>max value : <em>float,</em></strong> is of the same data type and structure as the elements in array.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Array_Integer_32.Png" src="assets/output_array_integer_32.png" width="42"/></td>
      <td valign="top"><strong>max index(es) : <em>array,</em></strong> index for the first max value. If array is multidimensional, max index(es) is an array whose elements are the indexes for the first maximum value in array.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Single.Png" src="assets/output_single.png" width="42"/></td>
      <td valign="top"><strong>min value : <em>float,</em></strong> is of the same data type and structure as the elements in array.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Array_Integer_32.Png" src="assets/output_array_integer_32.png" width="42"/></td>
      <td valign="top"><strong>min index(es) : <em>array,</em></strong> index for the first max value. If array is multidimensional, max index(es) is an array whose elements are the indexes for the first minimum value in array.</td>
    </tr>
  </tbody>
</table>

<h2>Examples</h2>

<p>All these examples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Accelerator library to run it).</p>

<p align="center"><img src="assets/ex_min_and_max.png" alt="ex_min_and_max" width="260" /></p>
