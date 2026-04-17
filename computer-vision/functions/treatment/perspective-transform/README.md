<h1>Perspective Transform</h1>

<h2>Description</h2>

<p>Calculates a perspective transform from four pairs of the corresponding points. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="Perspective Transform" src="assets/Perspective Transform.png" width="341"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Image_Src.Png" src="assets/input_image_src.png" width="42"/></td>
      <td valign="top"><strong>Image Src : <em>class, </em></strong>type accepted <strong>U8</strong>, <strong>I16</strong>, <strong>RGB</strong> and <strong>HSL.</strong></td>
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
      <td valign="top"><strong>PerspectiveTransform Parameters :<em> cluster,</em></strong></td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Array_Cluster_1.Png" src="assets/input_array_cluster_1.png" width="42"/></td>
      <td valign="top"><strong>Src Point : <em>array, </em></strong>coordinates of quadrangle vertices in the source image.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Array_Cluster_1.Png" src="assets/input_array_cluster_1.png" width="42"/></td>
      <td valign="top"><strong>Dst Point : <em>array, </em></strong>coordinates of the corresponding quadrangle vertices in the destination image.</td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img src="assets/perspective_transform_param.png" alt="perspective_transform_param" width="260" /></p></td>
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
