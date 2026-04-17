<h1>Convert Pytorch To ONNX</h1>

<h2>Description</h2>

<p>This VI uses a Python-based export pipeline to convert a PyTorch model saved as .pt (TorchScript) into a .onnx file. Input shapes and ranks must be provided to define the tracing inputs. The generated ONNX model can be optionally opened in Netron.</p>

<p align="center"><img alt="Pytorch To ONNX" src="assets/Pytorch To ONNX.png" width="220"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Booleen.Png" src="assets/booleen.png" width="42"/></td>
      <td valign="top"><strong>Open Netron : <em>boolean, </em></strong>indicating whether to automatically open the resulting ONNX file in Netron after conversion. If true opens in Netron else conversion only.</td>
    </tr>
  </tbody>
</table>

<table>
  <tbody>
    <tr>
      <td valign="top" width="70%"><p><img alt="Cluster.Png" src="assets/cluster.png" width="32"/><strong>Conversion Parameters : <em>cluster,</em></strong></p>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Path In.Png" src="assets/path-in.png" width="42"/></td>
      <td valign="top"><strong>ONNX Model Path : <em>path</em>, </strong>path where the ONNX file will be saved.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Path In.Png" src="assets/path-in.png" width="42"/></td>
      <td valign="top"><strong>Pytorch Model Path : <em>path</em>, </strong>path to the source PyTorch model file (TorchScript format).</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Array Integer 32.Png" src="assets/array-integer-32.png" width="42"/></td>
      <td valign="top"><strong>Shapes : <em>array, </em></strong>a flattened 1D array representing all input tensor shapes, concatenated. Each shape must be fully specified (e.g., <code>[1, 3, 224, 224, 1, 10]</code>).</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Array Integer 32.Png" src="assets/array-integer-32.png" width="42"/></td>
      <td valign="top"><strong>Ranks : <em>array, </em></strong>specifying the rank (number of dimensions) of each input tensor. This array is used to split the flat <code>Shapes</code> array into individual shapes for each input.</td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img alt="param_onnx_to_pytorch" src="assets/param_onnx_to_pytorch.png" width="220"/></p></td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="String Out.Png" src="assets/string-out.png" width="42"/></td>
      <td valign="top"><strong>standard output : <em>string, </em></strong>text output from the underlying Python process. Can include logs, conversion info, or warnings.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="String Out.Png" src="assets/string-out.png" width="42"/></td>
      <td valign="top"><strong>standard error : <em>string, </em></strong>text output capturing any error messages from the Python process, useful for debugging failed conversions.</td>
    </tr>
  </tbody>
</table>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>
