<h1>Get Image Info</h1>

<h2>Description</h2>

<p>Retrieve image information (name, size, and type). Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="Get Image Info" src="assets/Get Image Info.png" width="238"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Image_Src.Png" src="assets/input_image_src.png" width="42"/></td>
      <td valign="top"><strong>Image Src : <em>class</em></strong></td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_String.Png" src="assets/output_string.png" width="42"/></td>
      <td valign="top"><strong>Name : <em>string, </em></strong>image name.</td>
    </tr>
  </tbody>
</table>

<table>
  <tbody>
    <tr>
      <td valign="top" width="70%"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Cluster_1.Png" src="assets/output_cluster_1.png" width="42"/></td>
      <td valign="top"><strong>Image Info : <em>cluster,</em> </strong></td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Interger_32.Png" src="assets/output_interger_32.png" width="42"/></td>
      <td valign="top"><strong>Width :<em> integer, </em></strong>image width.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Interger_32.Png" src="assets/output_interger_32.png" width="42"/></td>
      <td valign="top"><strong>Height :<em> integer, </em></strong>image height.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Unsigned_32.Png" src="assets/output_unsigned_32.png" width="42"/></td>
      <td valign="top"><strong>Image Type : <em>integer, </em></strong>specifies the type of the image.
<ul>
<li>
<ul>
<li>
<ul>
<li>
<ul>
<li>Grayscale (U8) : 8 bits per pixel (unsigned, standard monochrome)</li>
<li>Grayscale (I16) : 16 bits per pixel (signed)</li>
<li>Grayscale (SGL) : 32 bits per pixel (floating point)</li>
<li>Complex (CSG) : 2 × 32 bits per pixel (floating point)</li>
<li>RGB (U32) : 32 bits per pixel (red, green, blue, alpha)</li>
<li>HSL (U32) : 32 bits per pixel (hue, saturation, luminance, alpha)</li>
<li>RGB (U64) : 64 bits per pixel (red, green, blue, alpha)</li>
<li>Grayscale (U16) : 16 bits per pixel (unsigned)</li>
</ul>
</li>
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
      <td valign="top" width="30%"><p align="center"><img src="assets/image_info.png" alt="image_info" width="114" /></p></td>
    </tr>
  </tbody>
</table>

<h2>Examples</h2>

<p>All these examples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Computer Vision ​library to run it).</p>
