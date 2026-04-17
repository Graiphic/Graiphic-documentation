<h1>Release Video Writer</h1>

<h2>Description</h2>

<p>Close the VideoWriter reference. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="ReleaseVideoWriter" src="assets/ReleaseVideoWriter.png" width="261"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Video_Writer.Png" src="assets/input_video_writer.png" width="42"/></td>
      <td valign="top"><strong>VideoWriter Src : <em>class</em></strong></td>
    </tr>
  </tbody>
</table>

<h2>Examples</h2>

<p>All these examples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Computer Vision library to run it).</p>

<h3>Create and write video</h3>

<p align="center"><img src="assets/video_writer_example.png" alt="video_writer_example" width="260" /></p>

<p>1 – Initialize</p>

<p>Open camera reference, create a temporary memory location for an image and create video reference.</p>

<p>2 – Process</p>

<p>Each loop reads the last frame and displays this frame. If the “Record” boolean is true, the image is saved in video.</p>

<p>3 – Close</p>

<p>We close all open references.</p>
