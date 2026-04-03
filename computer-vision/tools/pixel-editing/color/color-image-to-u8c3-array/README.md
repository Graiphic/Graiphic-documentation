<h1>Color Image To U8C3 Array</h1>

<h2>Description</h2>

<p>Extracts the pixels from a color image or from part of a color image into a U8 3D array. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img src="assets/color_image_to_u8c3_array.png" alt="Color_Image_To_U8C3_Array.Png" width="264" /></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Image_Src.Png" src="assets/input_image_src.png" width="42"/></td>
      <td valign="top"><strong>Image Src : <em>class, </em></strong>type accepted <strong>RGB</strong> and <strong>HSL</strong>.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Enum.Png" src="assets/input_enum.png" width="42"/></td>
      <td valign="top">Array Type :<em> enum, </em>define the dimension order.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Enum.Png" src="assets/input_enum.png" width="42"/></td>
      <td valign="top"><strong>Color Order : <em>enum</em>, </strong>define the Red/Blue/Green channel Order in the output image.</td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Image_Src.Png" src="assets/output_image_src.png" width="42"/></td>
      <td valign="top"><strong>Dup Image Src :<em> class</em></strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Array_Unsigned_8_.Png" src="assets/output_array_unsigned_8_.png" width="42"/></td>
      <td valign="top">Image Array :<em> array, </em>returns the pixel values as a 3D array of unsigned 8-bit integers.</td>
    </tr>
  </tbody>
</table>

<h2>Examples</h2>

<p>All these examples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Computer Vision ​library to run it).</p>
