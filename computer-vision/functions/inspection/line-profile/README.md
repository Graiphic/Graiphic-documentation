<h1>Line Profile</h1>

<h2>Description</h2>

<p>Calculates the profile of a line of pixels. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img src="assets/line_profile.png" alt="Line_Profile.Png" width="313" /></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Image_Src.Png" src="assets/input_image_src.png" width="42"/></td>
      <td valign="top"><strong>Image Src : <em>class, </em></strong>type accepted <strong>U8</strong> and <strong>I16</strong>.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Array_Integer_32.Png" src="assets/input_array_integer_32.png" width="42"/></td>
      <td valign="top"><strong>Line Coordinates : <em>array, </em></strong>specifying the pixel coordinates that form the end points of the line.</td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td valign="top" width="70%"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Cluster_2.Png" src="assets/output_cluster_2.png" width="42"/></td>
      <td valign="top"><strong>Line Graph : <em>cluster, </em></strong>contains the line profile with an x-origin at 0 and an increment of 1.</td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Interger_32.Png" src="assets/output_interger_32.png" width="42"/></td>
      <td valign="top"><strong>x0 : <em>integer, </em></strong>always returns 0.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Interger_32.Png" src="assets/output_interger_32.png" width="42"/></td>
      <td valign="top">dx :<em> integer, </em>always returns 1.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Array_Integer_32.Png" src="assets/output_array_integer_32.png" width="42"/></td>
      <td valign="top">Pixels Line :<em> array, </em>returns the line profile calculated in an array in which elements represent the pixel values belonging to the specified vector.</td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img src="assets/line_graph.png" alt="line_graph" width="153" /></p></td>
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
      <td valign="top"><strong>ROI Pixel Statistics : <em>cluster, </em></strong>contains relevant information about the pixels found in the specified vector.</td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Interger_32.Png" src="assets/output_interger_32.png" width="42"/></td>
      <td valign="top"><strong>Min : <em>integer, </em></strong>returns the smallest pixel value found in the line profile.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Interger_32.Png" src="assets/output_interger_32.png" width="42"/></td>
      <td valign="top">Max :<em> integer, </em>returns the largest pixel value found in the line profile.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Double.Png" src="assets/output_double.png" width="42"/></td>
      <td valign="top">Mean :<em> float, </em>returns the mean value of the pixels found in the line profile.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Double.Png" src="assets/output_double.png" width="42"/></td>
      <td valign="top">Std Dev :<em> float, </em>returns the standard deviation from the line profile.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Interger_32.Png" src="assets/output_interger_32.png" width="42"/></td>
      <td valign="top">Count :<em> integer, </em>returns the number of pixels found in the line profile.</td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img src="assets/roi_pixel_statistics.png" alt="roi_pixel_statistics" width="99" /></p></td>
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
      <td valign="top"><strong>Global Rectangle : <em>cluster, </em></strong>contains the coordinates of a bounding rectangle for the line in the image.</td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Interger_32.Png" src="assets/output_interger_32.png" width="42"/></td>
      <td valign="top"><strong>Left : </strong>integer, indicates the x-coordinate of the top-left corner of the rectangle.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Interger_32.Png" src="assets/output_interger_32.png" width="42"/></td>
      <td valign="top">Top : integer, indicates the y-coordinate of the top-left corner of the rectangle.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Interger_32.Png" src="assets/output_interger_32.png" width="42"/></td>
      <td valign="top">Right : integer, indicates the x-coordinate of the bottom-right corner of the rectangle.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Interger_32.Png" src="assets/output_interger_32.png" width="42"/></td>
      <td valign="top">Bottom : integer, indicates the y-coordinate of the bottom-right corner of the rectangle.</td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img src="assets/global_rectangle.png" alt="global_rectangle" width="92" /></p></td>
    </tr>
  </tbody>
</table>

<h2>Examples</h2>

<p>All these examples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Computer Vision ​library to run it).</p>
