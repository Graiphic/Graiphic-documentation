<h1>Canny Edge Detection</h1>

<h2>Description</h2>

<p>Uses a specialized edge detection method to accurately estimate the location of edges even under conditions of poor signal-to-noise ratios. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="Canny Edge Detection" src="assets/Canny Edge Detection.png" width="274"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Image_Src.Png" src="assets/input_image_src.png" width="42"/></td>
      <td valign="top"><strong>Image Src : <em>class, </em></strong>type accepted<strong> U8 </strong>and<strong> I16.</strong></td>
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
      <td valign="top"><strong>Canny Parameters :<em> cluster,</em></strong></td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Double.Png" src="assets/input_double.png" width="42"/></td>
      <td valign="top"><strong>Lower Threshold : <em>float, </em></strong>first threshold for the hysteresis procedure.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Double.Png" src="assets/input_double.png" width="42"/></td>
      <td valign="top"><strong>Higher Threshold : <em>float, </em></strong>second threshold for the hysteresis procedure.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Interger_32.Png" src="assets/input_interger_32.png" width="42"/></td>
      <td valign="top">Kernel Size<em> : integer, </em>aperture size for the Sobel operator.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Boolean.Png" src="assets/input_boolean.png" width="42"/></td>
      <td valign="top"><strong>L2 Gradient : <em>boolean, </em></strong>a flag, indicating whether a more accurate L2 norm should be used to calculate the image gradient magnitude ( L2gradient=true ), or whether the default L1 norm is enough ( L2gradient=false ).</td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img src="assets/canny_param.png" alt="canny_param" width="99" /></p></td>
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
