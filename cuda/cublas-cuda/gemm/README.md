<h1>gemm</h1>

<h2>Description</h2>

<p>This function performs the matrix-matrix multiplication : C = α * op(A) * op(B) + β * C<br/>Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img src="assets/gemm.png" alt="Gemm.Png" width="209" /></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Tensor.Png" src="assets/input_tensor.png" width="42"/></td>
      <td valign="top"><strong>A : <em>class, </em></strong>2D tensor of dimension M x K.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Tensor.Png" src="assets/input_tensor.png" width="42"/></td>
      <td valign="top"><strong>B : <em>class, </em></strong>2D tensor of dimension K x N.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Tensor.Png" src="assets/input_tensor.png" width="42"/></td>
      <td valign="top"><strong>C : <em>class, </em></strong>2D tensor of dimension M x N.</td>
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
      <td width="64" valign="top"><img alt="Input_Enum.Png" src="assets/input_enum.png" width="42"/></td>
      <td valign="top"><strong>Op(B) : <em>enum,</em></strong> operation that is non- or transpose.
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
      <td valign="top"><strong>β : <em>float,</em></strong> scalar used for multiplication, if beta==0 then C does not have to be a valid input.</td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Tensor.Png" src="assets/output_tensor.png" width="42"/></td>
      <td valign="top"><strong>C : <em>class, </em></strong>2D tensor of dimension M x N.</td>
    </tr>
  </tbody>
</table>

<h2>Examples</h2>

<p>All these examples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Accelerator library to run it).</p>

<h3>The non-transposed operation is selected for A and B</h3>

<p align="center"><img src="assets/ex_gemm_non_transpose.png" alt="ex_gemm_non_transpose" width="260" /></p>

<h3>The transposed operation is selected for A and B</h3>

<p align="center"><img src="assets/ex_gemm_transpose.png" alt="ex_gemm_transpose" width="260" /></p>

<h3>The transposed operation is selected for B</h3>

<p align="center"><img src="assets/ex_gemm_transpose_for_b.png" alt="ex_gemm_transpose_for_b" width="260" /></p>

<h3>The transposed operation is selected for A</h3>

<p align="center"><img src="assets/ex_gemm_transpose_for_a.png" alt="ex_gemm_transpose_for_a" width="260" /></p>
