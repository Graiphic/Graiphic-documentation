<h1>Set Color Pixel Line</h1>

<h2>Description</h2>

<p>Changes a line of pixels from a color image. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img src="assets/set_color_pixel_line.png" alt="Set_Color_Pixel_Line.Png" width="269" /></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Image_Src.Png" src="assets/input_image_src.png" width="42"/></td>
      <td valign="top"><strong>Image Src : <em>class, </em></strong>type accepted <strong>RGB</strong> and <strong>HSL</strong>.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Array_Integer_32.Png" src="assets/input_array_integer_32.png" width="42"/></td>
      <td valign="top">Line Coordinates : <em>array, </em>array specifying the pixel coordinates that form the endpoints of the line to modify. Any coordinates located outside the actual image are not used.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Array_Unsigned_32.Png" src="assets/input_array_unsigned_32.png" width="42"/></td>
      <td valign="top"><strong>Pixels Line (U32) : <em>array, </em></strong>contains the pixel values as a 1D array of unsigned 32-bit integers.</td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Image_Src.Png" src="assets/output_image_src.png" width="42"/></td>
      <td valign="top"><strong>Image Src :<em> class</em></strong></td>
    </tr>
  </tbody>
</table>

<h2>Examples</h2>

<p>All these examples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Computer Vision ​library to run it).</p>
