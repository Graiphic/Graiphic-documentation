<h1>Rotate</h1>

<h2>Description</h2>

<p>Rotates an image. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="Rotate" src="assets/Rotate.png" width="274"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Image_Src.Png" src="assets/input_image_src.png" width="42"/></td>
      <td valign="top"><strong>Image Src : <em>class, </em></strong>type accepted <strong>U8</strong>, <strong>I16</strong>, <strong>RGB</strong> and <strong>HSL</strong>.</td>
    </tr>
  </tbody>
</table>

<table>
  <tbody>
    <tr>
      <td valign="top" width="70%"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Cluster_1.Png" src="assets/input_cluster_1.png" width="42"/></td>
      <td valign="top"><strong>Rotate Parameters :<em> cluster,</em></strong></td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Double.Png" src="assets/input_double.png" width="42"/></td>
      <td valign="top"><strong>Angle : <em>float, </em></strong>defines the angle to rotate.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Enum.Png" src="assets/input_enum.png" width="42"/></td>
      <td valign="top">Interpolation :<em> enum,</em>
<ul>
<li>
<ul>
<li>
<ul>
<li>NEAREST : nearest neighbor interpolation.</li>
<li>LINEAR : bilinear interpolation.</li>
<li>CUBIC : bicubic interpolation.</li>
<li>AREA : resampling using pixel area relation. It may be a preferred method for image decimation, as it gives moire’-free results. But when the image is zoomed, it is similar to the INTER_NEAREST method.</li>
<li>LANCZOS4 : Lanczos interpolation over 8×8 neighborhood.</li>
</ul>
</li>
</ul>
</li>
</ul></td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img src="assets/rotate_param.png" alt="rotate_param" width="195" /></p></td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Image_Src.Png" src="assets/output_image_src.png" width="42"/></td>
      <td valign="top"><strong>Image Dst : <em>class</em></strong></td>
    </tr>
  </tbody>
</table>

<h2>Examples</h2>

<p>All these examples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Computer Vision ​library to run it).</p>
