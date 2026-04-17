<h1>Open Camera</h1>

<h2>Description</h2>

<p>Opens camera reference according to index. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="Open Camera" src="assets/Open Camera.png" width="225"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Unsigned_16.Png" src="assets/input_unsigned_16.png" width="42"/></td>
      <td valign="top"><strong>Camera : <em>integer, </em></strong>camera index.</td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Session.Png" src="assets/output_session.png" width="42"/></td>
      <td valign="top"><strong>Session Dst : <em>class</em></strong></td>
    </tr>
  </tbody>
</table>

<h2>Examples</h2>

<p><a href="https://www.youtube.com/embed/dLkRw9v3Z6Y?feature=oembed">Get started - Open a camera with TIGR vision toolkit for LabVIEW</a></p>

<p>All these examples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Computer Vision library to run it).</p>

<h3>Open and play a camera with LabVIEW picture display</h3>

<p align="center"><img src="assets/read_camera.png" alt="read_camera" width="260" /></p>

<p>1 – Initialize</p>

<p>Open camera reference and create a temporary memory allocation for an image.</p>

<p>2 – Process</p>

<p>Each loop reads the last frame and displays this frame.</p>

<p>3 – Close</p>

<p>We close all open references.</p>

<h3>Open and play a camera with CV display</h3>

<p align="center"><img src="assets/play_camera.png" alt="play_camera" width="260" /></p>

<p>1 – Initialize</p>

<p>Open camera reference and create a temporary memory allocation for an image.</p>

<p>2 – Process</p>

<p>Each loop reads the last frame and displays this frame.</p>

<p>3 – Close</p>

<p>We close all open references.</p>
