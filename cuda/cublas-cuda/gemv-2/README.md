<h1>gemv</h1>

<h2>Description</h2>

<p>This function performs the matrix-vector multiplication : y = α * op(A)x + β * y<br/>Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img src="assets/gemv.png" alt="Gemv.Png" width="209" /></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Tensor.Png" src="assets/input_tensor.png" width="42"/></td>
      <td valign="top"><strong>A : <em>class, </em></strong>2D tensor of dimension N x M.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Tensor.Png" src="assets/input_tensor.png" width="42"/></td>
      <td valign="top"><strong>x : <em>class, </em></strong>1D tensor of dimension M.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Tensor.Png" src="assets/input_tensor.png" width="42"/></td>
      <td valign="top"><strong>y : <em>class, </em></strong>1D tensor of dimension N. The default is an N-element vector with all elements equal to 0.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Enum.Png" src="assets/input_enum.png" width="42"/></td>
      <td valign="top"><strong>Op(A) : <em>enum,</em></strong> operation that is non- or transpose.
<ul>
<li>
<ul>
<li>CUBLAS_OP_N : the non-transpose operation is selected</li>
<li>CUBLAS_OP_T : the transpose operation is selected</li>
<li>CUBLAS_OP_H : the conjugate transpose operation is selected</li>
</ul>
</li>
</ul></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Single.Png" src="assets/input_single.png" width="42"/></td>
      <td valign="top"><strong>α : <em>float,</em></strong> scalar used for multiplication.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Single.Png" src="assets/input_single.png" width="42"/></td>
      <td valign="top"><strong>β : <em>float,</em></strong> scalar used for multiplication, if beta==0 then y does not have to be a valid input.</td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Tensor.Png" src="assets/output_tensor.png" width="42"/></td>
      <td valign="top"><strong>y : <em>class, </em></strong>1D tensor of dimension N.</td>
    </tr>
  </tbody>
</table>

<h2>Examples</h2>

<p>All these examples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Accelerator library to run it).</p>

<h3>NON-TRANSPOSE</h3>

<p align="center"><img src="assets/ex_gemv_non_transpose.png" alt="ex_gemv_non_transpose" width="260" /></p>

<h3>TRANSPOSE</h3>

<p align="center"><img src="assets/ex_gemv_transpose.png" alt="ex_gemv_transpose" width="260" /></p>
