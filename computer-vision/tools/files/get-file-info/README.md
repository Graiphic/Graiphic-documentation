<h1>Get File Info</h1>

<h2>Description</h2>

<p>Obtains information regarding the contents of the file. This information is supplied for standard file formats only : BMP, TIFF, JPEG, JPEG2000, PNG, or AIPD. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img src="assets/get_file_info.png" alt="Get_File_Info.Png" width="229" /></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Path.Png" src="assets/input_path.png" width="42"/></td>
      <td valign="top"><strong>File Path : <em>path, </em></strong>file path (BMP, TIFF, JPEG, JPEG2000, PNG, AIPD).</td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_String.Png" src="assets/output_string.png" width="42"/></td>
      <td valign="top"><strong>File Type :<em> string, </em></strong>file extension.</td>
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
      <td valign="top"><strong>File Info : <em>cluster,</em> </strong></td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Interger_32.Png" src="assets/output_interger_32.png" width="42"/></td>
      <td valign="top"><strong>Width :<em> integer, </em></strong>image width.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Interger_32.Png" src="assets/output_interger_32.png" width="42"/></td>
      <td valign="top"><strong>Height :<em> integer, </em></strong>image height.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Unsigned_32.Png" src="assets/output_unsigned_32.png" width="42"/></td>
      <td valign="top"><strong>Image Type : <em>integer, </em></strong>specifies the type of the image.
<ul>
<li>
<ul>
<li>
<ul>
<li>
<ul>
<li>
<ul>
<li>Grayscale (U8) : 8 bits per pixel (unsigned, standard monochrome)</li>
<li>Grayscale (I16) : 16 bits per pixel (signed)</li>
<li>Grayscale (SGL) : 32 bits per pixel (floating point)</li>
<li>Complex (CSG) : 2 × 32 bits per pixel (floating point)</li>
<li>RGB (U32) : 32 bits per pixel (red, green, blue, alpha)</li>
<li>HSL (U32) : 32 bits per pixel (hue, saturation, luminance, alpha)</li>
<li>RGB (U64) : 64 bits per pixel (red, green, blue, alpha)</li>
<li>Grayscale (U16) : 16 bits per pixel (unsigned)</li>
</ul>
</li>
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
      <td valign="top" width="30%"><p align="center"><img src="assets/file_info.png" alt="file_info" width="114" /></p></td>
    </tr>
  </tbody>
</table>

<h2>Examples</h2>

<p>All these examples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Computer Vision ​library to run it).</p>
