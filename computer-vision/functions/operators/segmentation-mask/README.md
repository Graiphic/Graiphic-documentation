<h1>Segmentation Mask</h1>

<h2>Description</h2>

<p>The Segmentation Mask function merges a base image with a color mask using a given opacity factor, producing a partially masked image. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="Segmentation Mask" src="assets/Segmentation Mask.png" width="279"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Image_Src.Png" src="assets/input_image_src.png" width="42"/></td>
      <td valign="top"><strong>Image Src : <em>class, </em></strong>type accepted <strong>RGB</strong> and <strong>HSL</strong>.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Image_Src.Png" src="assets/input_image_src.png" width="42"/></td>
      <td valign="top"><strong>Image Mask : <em>class, </em></strong>type accepted <strong>RGB</strong> and <strong>HSL</strong>.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Single.Png" src="assets/input_single.png" width="42"/></td>
      <td valign="top">Mask Transparency : <em>float, </em>parameter defining the transparency of masks on the original image. From 0 = opaque to 1 = transparent.</td>
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
