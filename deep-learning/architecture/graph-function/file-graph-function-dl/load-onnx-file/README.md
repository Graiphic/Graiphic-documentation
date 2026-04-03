<h1>Load ONNX File</h1>

<h2>Description</h2>

<p>Loads an ONNX model from file and creates the corresponding execution graph.<br/>
This VI initializes an ONNXModel object from a .onnx file, making it ready for use within the Deep Learning environment. It allows importing external models into the LabVIEW graphical workflow, with an optional loading popup.</p>

<p align="center"><img alt="load_model_and_create_graph" src="assets/load_model_and_create_graph.png" width="220"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Path In.Png" src="assets/path-in.png" width="42"/></td>
      <td valign="top"><strong>File Path : <em>path</em>,</strong> path to the <code>.onnx</code> file to be loaded. The file must contain a valid ONNX graph.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Booleen.Png" src="assets/booleen.png" width="42"/></td>
      <td valign="top"><strong>Display Loading Popup : <em>boolean, </em></strong>indicating whether to show a loading popup during model import. If true, shows a loading window else, loads the model silently in the background.</td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Object_3.Png" src="assets/output_object_3.png" width="42"/></td>
      <td valign="top"><strong>ONNX out : </strong>reference to the loaded ONNX model, encapsulated in the <code>ONNXModel</code> class of the Deep Learning toolkit. Functionally equivalent to a model built manually from nodes.</td>
    </tr>
  </tbody>
</table>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>
