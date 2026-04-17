<h1>Extract Color Planes</h1>

<h2>Description</h2>

<p>Extracts the three planes (RGB, HSL, HSV, or HSI) from an image. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="Extract Color Planes" src="assets/Extract Color Planes.png" width="357"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Image_Src.Png" src="assets/input_image_src.png" width="42"/></td>
      <td valign="top"><strong>Image Src : <em>class, </em></strong>type accepted <strong>RGB</strong> and <strong>HSL</strong>.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Enum.Png" src="assets/input_enum.png" width="42"/></td>
      <td valign="top">Target Type :<em> enum, </em>defines the image color format to use for the operation.
<ul>
<li>
<ul>
<li>RGB : specifies the color format RGB (red, green, and blue)</li>
<li>HSL : specifies the color format HSI (hue, saturation, and luminance)</li>
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
      <td valign="top"><strong>Red/Hue : <em>class, </em></strong>reference to the image containing the red (or hue) plane of the source (input) image.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Image_Src.Png" src="assets/output_image_src.png" width="42"/></td>
      <td valign="top">Green/Saturation : <em>class, </em>reference to the image containing the green (or saturation) plane of the source (input) image.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Image_Src.Png" src="assets/output_image_src.png" width="42"/></td>
      <td valign="top">Blue/Luminance/Value/Intensity : <em>class, </em>reference to the image containing the blue (or luminance, value, or intensity) plane of the source (input) image.</td>
    </tr>
  </tbody>
</table>

<h2>Examples</h2>

<p>All these examples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Computer Vision ​library to run it).</p>
