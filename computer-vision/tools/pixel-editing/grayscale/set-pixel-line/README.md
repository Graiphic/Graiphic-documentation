<h1>Set Pixel Line</h1>

<h2>Description</h2>

<p>Changes the intensity values in a line of pixels of an image. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img src="assets/set_pixel_line.png" alt="Set_Pixel_Line.Png" width="269" /></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Image_Src.Png" src="assets/input_image_src.png" width="42"/></td>
      <td valign="top"><strong>Image Src : <em>class, </em></strong>type accepted <strong>U8</strong> and <strong>I16</strong>.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Array_Integer_32.Png" src="assets/input_array_integer_32.png" width="42"/></td>
      <td valign="top">Line Coordinates : <em>array, </em>four-element array specifying the pixel coordinates that form the end points of the line to modify. The first two elements (left, top) in the array correspond to the coordinates for the first endpoint of the line. The last two elements (right, bottom) correspond to the second endpoint of the line.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Array_Unsigned_8.Png" src="assets/input_array_unsigned_8.png" width="42"/></td>
      <td valign="top"><strong>Pixels Line (U8) : <em>array, </em></strong>array of unsigned 8-bit integers containing the new values for the pixel line. This input is required if Image is an unsigned 8-bit image.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Array_Integer_16.Png" src="assets/input_array_integer_16.png" width="42"/></td>
      <td valign="top"><strong>Pixels Line (I16) : <em>array, </em></strong>array of 16-bit integers containing the new values for the pixel line. This input is required if Image is an 16-bit image.</td>
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
