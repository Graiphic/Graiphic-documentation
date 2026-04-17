<h1>Normalize</h1>

<h2>Description</h2>

<p>Normalizes the norm or value range of an array. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="Normalize" src="assets/Normalize.png" width="294"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Image_Src.Png" src="assets/input_image_src.png" width="42"/></td>
      <td valign="top"><strong>Image Src : <em>class,</em></strong> type accepted <strong>U8</strong>, <strong>I16</strong>, <strong>RGB</strong> and <strong>HSL.</strong></td>
    </tr>
  </tbody>
</table>

<table>
  <tbody>
    <tr>
      <td valign="top" width="70%"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Cluster_1.Png" src="assets/input_cluster_1.png" width="42"/></td>
      <td valign="top"><strong>Normalize Parameters :<em> cluster,</em></strong></td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Double.Png" src="assets/input_double.png" width="42"/></td>
      <td valign="top"><strong>Alpha : <em>float, </em></strong>norm value to normalize to or the lower range boundary in case of the range normalization.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Double.Png" src="assets/input_double.png" width="42"/></td>
      <td valign="top">Beta : <em>float, </em>upper range boundary in case of the range normalization; it is not used for the norm normalization.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Unsigned_16.Png" src="assets/input_unsigned_16.png" width="42"/></td>
      <td valign="top">Norm Type :<em> integer, </em>normalization type.</td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table>

<p>NORM_INF</p>

<p align="center"><img src="assets/norm_inf.png" alt="Norm_Inf.Png" width="460" /></p>

<p>NORM_L1</p>

<p align="center"><img src="assets/norm_l1.png" alt="Norm_L1.Png" width="460" /></p>

<p>NORM_L2</p>

<p align="center"><img src="assets/norm_l2.png" alt="Norm_L2.Png" width="460" /></p>

<p>NORM_MINMAX</p>

<p>flag</p></td>
      <td valign="top" width="30%"><p align="center"><img src="assets/norm_param.png" alt="norm_param" width="124" /></p></td>
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
