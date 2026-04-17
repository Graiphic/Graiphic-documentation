<h1>User Lookup</h1>

<h2>Description</h2>

<p>Performs a user-specified lookup-table transformation by remapping the pixel values in an image. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="User Lookup" src="assets/User Lookup.png" width="252"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Image_Src.Png" src="assets/input_image_src.png" width="42"/></td>
      <td valign="top"><strong>Image Src : <em>class, </em></strong>type accepted <strong>U8</strong> and <strong>I16</strong>.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Image_Src.Png" src="assets/input_image_src.png" width="42"/></td>
      <td valign="top">Image Mask : <em>class, </em>type accepted <strong>U8</strong> and <strong>I16</strong>.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Array_Integer_32.Png" src="assets/input_array_integer_32.png" width="42"/></td>
      <td valign="top">Lookup Table :<em> array, </em>is a grayscale replacement table. This input is an array containing a maximum of 256 elements if <strong>Image Src</strong> is an 8-bit image or a maximum of 65,536 elements if <strong>Image Src</strong> is a 16-bit image. Individual pixels within the image are not modified when the lookup table is missing a value that corresponds to those pixels.</td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Image_Src.Png" src="assets/output_image_src.png" width="42"/></td>
      <td valign="top"><strong>Image Dst :<em> class</em></strong></td>
    </tr>
  </tbody>
</table>

<h2>Examples</h2>

<p>All these examples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Computer Vision ​library to run it).</p>
