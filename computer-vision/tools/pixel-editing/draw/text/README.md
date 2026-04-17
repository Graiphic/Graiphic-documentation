<h1>Draw Text</h1>

<h2>Description</h2>

<p>Draw text in an image. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="Text" src="assets/Text.png" width="262"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Image_Src.Png" src="assets/input_image_src.png" width="42"/></td>
      <td valign="top"><strong>Image Src : <em>class, </em></strong>type accepted <strong>U8</strong>, <strong>I16</strong>, <strong>RGB</strong> and <strong>HSL</strong>.</td>
    </tr>
  </tbody>
</table>

<table>
  <tbody>
    <tr>
      <td valign="top" width="70%"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Cluster_2.Png" src="assets/input_cluster_2.png" width="42"/></td>
      <td valign="top"><strong>Text Parameters : <em>cluster</em></strong></td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_String.Png" src="assets/input_string.png" width="42"/></td>
      <td valign="top"><strong>Text : <em>string, </em></strong>text string to be drawn.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Interger_32.Png" src="assets/input_interger_32.png" width="42"/></td>
      <td valign="top">X :<em> integer, </em>X coordinate of the text string in the image.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Interger_32.Png" src="assets/input_interger_32.png" width="42"/></td>
      <td valign="top">Y :<em> integer, </em>Y coordinate of the text string in the image.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Enum.Png" src="assets/input_enum.png" width="42"/></td>
      <td valign="top">Font Face :<em> enum, </em>font type.
<ul>
<li>
<ul>
<li>
<ul>
<li>FONT_HERSHEY_SIMPLEX : normal size sans-serif font</li>
<li>FONT_HERSHEY_PLAIN : small size sans-serif font</li>
<li>FONT_HERSHEY_DUPLEX : normal size sans-serif font (more complex than FONT_HERSHEY_SIMPLEX)</li>
<li>FONT_HERSHEY_COMPLEX : normal size serif font</li>
<li>FONT_HERSHEY_TRIPLEX : normal size serif font (more complex than FONT_HERSHEY_COMPLEX)</li>
<li>FONT_HERSHEY_COMPLEX_SMALL : smaller version of FONT_HERSHEY_COMPLEX</li>
<li>FONT_HERSHEY_SCRIPT_SIMPLEX : hand-writing style font</li>
<li>FONT_HERSHEY_SCRIPT_COMPLEX : more complex variant of FONT_HERSHEY_SCRIPT_SIMPLEX</li>
</ul>
</li>
</ul>
</li>
</ul></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Double.Png" src="assets/input_double.png" width="42"/></td>
      <td valign="top"><strong>Font Scale : <em>float, </em></strong>font scale factor that is multiplied by the font-specific base size.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Unsigned_32.Png" src="assets/input_unsigned_32.png" width="42"/></td>
      <td valign="top">Text Color :<em> integer, </em>color of the text.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Unsigned_32.Png" src="assets/input_unsigned_32.png" width="42"/></td>
      <td valign="top"><strong>BG Color : <em>integer, </em></strong>background color of the text overlay.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Interger_32.Png" src="assets/input_interger_32.png" width="42"/></td>
      <td valign="top"><strong>Thickness : <em>integer, </em></strong>thickness of the lines used to draw a text.</td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img src="assets/text_param.png" alt="text_param" width="216" /></p></td>
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
