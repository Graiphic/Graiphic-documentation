<h1>Scale By Power Of Two</h1>

<h2>Description</h2>

<p>Multiplies x by 2 raised to the power of n.</p>

<p align="center"><img src="assets/scale_by_power_of_two.png" alt="Scale_By_Power_Of_Two.Png" width="164" /></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Interger_32.Png" src="assets/input_interger_32.png" width="42"/></td>
      <td valign="top"><strong>n : <em>integer,</em></strong> scalar number. This function rounds n before it scales x (0.5 rounds to 0; 0.51 rounds to 1).</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Tensor.Png" src="assets/input_tensor.png" width="42"/></td>
      <td valign="top"><strong>x : <em>class, </em></strong>n-dimensional tensor.</td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Tensor.Png" src="assets/output_tensor.png" width="42"/></td>
      <td valign="top"><strong>x*2^n : <em>class,</em></strong> the result of multiplying x by 2, raised to the power of n.</td>
    </tr>
  </tbody>
</table>

<h2>Examples</h2>

<p>All these examples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Accelerator library to run it).</p>

<p align="center"><img src="assets/ex_scale_by_power_of_two.png" alt="ex_scale_by_power_of_two" width="260" /></p>
