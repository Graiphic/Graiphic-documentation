<h1>Fill Hole</h1>

<h2>Description</h2>

<p>Fills the holes found in a particle. The holes are filled with a pixel value of 1. The source image must be an 8-bit binary image. The holes found in contact with the image border are never filled because it is impossible to determine whether these holes are part of a particle. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="Fill Hole" src="assets/Fill Hole.png" width="282"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Image_Src.Png" src="assets/input_image_src.png" width="42"/></td>
      <td valign="top"><strong>Image Src : <em>class, </em></strong>type accepted <strong>U8</strong>.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Boolean.Png" src="assets/input_boolean.png" width="42"/></td>
      <td valign="top">Connectivity 4/8 (8) :<em> boolean, </em>specifies the type of connectivity used by the algorithm for particle detection. The connectivity mode directly determines whether an adjacent pixel belongs to the same particle or a different particle.
<ul>
<li>
<ul>
<li>True : particle detection is performed in connectivity mode 8</li>
<li>False : particle detection is performed in connectivity mode 4</li>
</ul>
</li>
</ul></td>
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
