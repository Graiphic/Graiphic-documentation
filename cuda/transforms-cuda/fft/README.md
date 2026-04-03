<h1>FFT</h1>

<h2>Description</h2>

<p>Executes a single-precision real-to-complex, implicitly forward, cuFFT transform plan. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p><strong>Warning : A new tensor is created for the output. </strong></p>

<p align="center"><img src="assets/fft.png" alt="Fft.Png" width="209" /></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Tensor.Png" src="assets/input_tensor.png" width="42"/></td>
      <td valign="top"><strong>x : <em>class, </em></strong>tensor to the real input data (in GPU memory) to transform.</td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Tensor.Png" src="assets/output_tensor.png" width="42"/></td>
      <td valign="top"><strong>y : <em>class, </em></strong>contains the complex Fourier coefficients.</td>
    </tr>
  </tbody>
</table>

<h2>Examples</h2>

<p>All these examples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Accelerator library to run it).</p>

<p align="center"><img src="assets/ex_fft_and_ifft.png" alt="ex_fft_and_ifft" width="260" /></p>
