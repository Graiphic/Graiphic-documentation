<h1>Convert ONNX To H5</h1>

<h2>Description</h2>

<p>This VI transforms a .onnx model into the HDF5 format (.h5) commonly used in TensorFlow/Keras workflows. It enables ONNX models to be reused in training or inference pipelines within the Keras ecosystem. Optionally, the converted model can be visualized in Netron.</p>

<p align="center"><img alt="ONNX To H5" src="assets/ONNX To H5.png" width="220"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Booleen.Png" src="assets/booleen.png" width="42"/></td>
      <td valign="top"><strong>Open Netron : <em>boolean, </em></strong>indicating whether to automatically open the resulting ONNX file in Netron after conversion. If true opens in Netron else conversion only.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Path In.Png" src="assets/path-in.png" width="42"/></td>
      <td valign="top"><strong>ONNX Model Path : <em>path</em>, </strong>path to the input <code>.onnx</code> file containing the model to be converted.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Path In.Png" src="assets/path-in.png" width="42"/></td>
      <td valign="top"><strong>H5 Model Path : <em>path</em>, </strong>path to the destination <code>.h5</code> file where the converted Keras model will be saved.</td>
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
