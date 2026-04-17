<h1>Or</h1>

<h2>Description</h2>

<p>Performs an OR or NOR operation on two images or an image and a constant. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="Or" src="assets/Or.png" width="245"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Image_Src.Png" src="assets/input_image_src.png" width="42"/></td>
      <td valign="top"><strong>Image Src A : <em>class, </em></strong>type accepted <strong>U8</strong>, <strong>I16</strong>, <strong>RGB</strong> and <strong>HSL</strong>.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Image_Src.Png" src="assets/input_image_src.png" width="42"/></td>
      <td valign="top">Image Src B : <em>class, </em>type accepted <strong>U8</strong>, <strong>I16</strong>, <strong>RGB</strong> and <strong>HSL<em>.</em></strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Interger_64.Png" src="assets/input_interger_64.png" width="42"/></td>
      <td valign="top">Constant :<em> integer, </em>value used for image-constant operations. Constant must be a RGB color value when <strong>Image Src A</strong> is a color image.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Boolean.Png" src="assets/input_boolean.png" width="42"/></td>
      <td valign="top">Or/Nor (Or) :<em> boolean, </em>specifies which logic operation the function performs. If set to TRUE, the result of the OR is inverted, producing a NOR. The default is FALSE, which specifies an OR operation.</td>
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
