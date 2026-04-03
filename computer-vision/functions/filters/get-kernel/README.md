<h1>Get Kernel</h1>

<h2>Description</h2>

<p>Reads a predefined kernel. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img src="assets/get_kernel.png" alt="Get_Kernel.Png" width="283" /></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Unsigned_16.Png" src="assets/input_unsigned_16.png" width="42"/></td>
      <td valign="top"><strong>Kernel Family : <em>enum, </em></strong>determines the type of matrix. This value corresponds to the thousandth unit in the researched code.
<ul>
<li>
<ul>
<li>Gradient : specifies the kernel family as gradient</li>
<li>Laplacian : specifies the kernel family as Laplacian</li>
<li>Smoothing : specifies the kernel family as smoothing</li>
<li>Gaussian : specifies the kernel family as Gaussian</li>
</ul>
</li>
</ul></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Interger_32.Png" src="assets/input_interger_32.png" width="42"/></td>
      <td valign="top"><strong>Kernel Size (3,5,…) :</strong> <em><strong>integer, </strong></em>determines the horizontal and vertical matrix size. The values are 3, 5, and 7, corresponding to the convolutions 3 × 3, 5 × 5, and 7 × 7 supplied in the matrix catalog. This value corresponds to the hundredth unit in the researched code.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Interger_32.Png" src="assets/input_interger_32.png" width="42"/></td>
      <td valign="top"><strong>Kernel Number :</strong> <em><strong>integer, </strong></em>is the matrix family number. It is a two-digit number, between 0 and n, belonging to a family and a size. A number of predefined matrices are available for each type and size.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Interger_32.Png" src="assets/input_interger_32.png" width="42"/></td>
      <td valign="top"><strong>Kernel Code :</strong> <em><strong>integer, </strong></em>is a code you can use to directly access a convolution matrix. Each code specifies a specific convolution matrix. You can use this input if it is connected and is not 0. The kernel located in the file then is transcribed into a 2D array that is available from the output Kernel. You can use the codes to specify a predefined kernel.</td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Single.Png" src="assets/output_single.png" width="42"/></td>
      <td valign="top"><strong>Divider : <em>float, </em></strong>is the normalization factor associated with the retrieved kernel.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Array_Single.Png" src="assets/output_array_single.png" width="42"/></td>
      <td valign="top">Kernel :<em> array, </em>resulting matrix. It corresponds to a kernel encoded by a code specified from the inputs <strong>Kernel Family</strong>, <strong>Kernel Size</strong>, and <strong>Kernel Number</strong> or a from a code directly passed through the input<strong> Kernel Code</strong>. You can connect this output directly to the input Kernel in the <a href="../convolute/README.md">Convolute</a> function.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Interger_32.Png" src="assets/output_interger_32.png" width="42"/></td>
      <td valign="top">Kernel code :<em> integer, </em>indicates the code that was used to retrieve the kernel.</td>
    </tr>
  </tbody>
</table>

<h2>Examples</h2>

<p>All these examples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Computer Vision ​library to run it).</p>
