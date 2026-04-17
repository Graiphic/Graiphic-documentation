<h1>Match Template</h1>

<h2>Description</h2>

<p>Search Image Template in Image Src and add bounding box to Image Dst where it is located. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="Match Template" src="assets/Match Template.png" width="286"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Image_Src.Png" src="assets/input_image_src.png" width="42"/></td>
      <td valign="top"><strong>Image Src : <em>class, </em></strong>type accepted <strong>U8</strong>.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Image_Src.Png" src="assets/input_image_src.png" width="42"/></td>
      <td valign="top"><strong>Image Template : <em>class, </em></strong>type accepted <strong>U8</strong>.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Single.Png" src="assets/input_single.png" width="42"/></td>
      <td valign="top">threshold : <em>float, </em>similarity coefficient between function results and template image.</td>
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

<table>
  <tbody>
    <tr>
      <td valign="top" width="70%"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Array_Cluster_1.Png" src="assets/output_array_cluster_1.png" width="42"/></td>
      <td valign="top"><strong>Detected Box : <em>cluster,</em></strong></td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Interger_32.Png" src="assets/output_interger_32.png" width="42"/></td>
      <td valign="top"><strong>left : <em>integer,</em></strong> left coordinate of box.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Interger_32.Png" src="assets/output_interger_32.png" width="42"/></td>
      <td valign="top"><strong>top : <em>integer,</em></strong> top coordinate of box.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Interger_32.Png" src="assets/output_interger_32.png" width="42"/></td>
      <td valign="top"><strong>right : <em>integer,</em></strong> right coordinate of box.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Interger_32.Png" src="assets/output_interger_32.png" width="42"/></td>
      <td valign="top"><strong>bottom : <em>integer,</em></strong> bottom coordinate of box.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Single.Png" src="assets/output_single.png" width="42"/></td>
      <td valign="top"><strong>threshold : <em>float,</em></strong> similarity coefficient of box.</td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img src="assets/detected_box.png" alt="detected_box" width="220" /></p></td>
    </tr>
  </tbody>
</table>

<h2>Examples</h2>

<p>All these examples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Computer Vision ​library to run it).</p>
