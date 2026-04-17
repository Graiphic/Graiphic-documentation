<h1>Auto Adjust Contrast</h1>

<h2>Description</h2>

<p>Boosts contrast based on the image’s histogram to improve normalization and line detection in varying lighting conditions. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="Auto Adjust Contrast" src="assets/Auto Adjust Contrast.png" width="234"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Image_Src.Png" src="assets/input_image_src.png" width="42"/></td>
      <td valign="top"><strong>Image Src : <em>class, </em></strong>type accepted <strong>U8</strong>, <strong>RGB</strong> and <strong>HSL</strong>.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Unsigned_16.Png" src="assets/input_unsigned_16.png" width="42"/></td>
      <td valign="top">Mode : <em>integer</em>, specifies the auto-tuning method :
<ul>
<li>
<ul>
<li>Contrast Stretching : Adjusts extreme pixel values to utilize the full grayscale range, enhancing overall contrast.</li>
<li>Histogram Equalization : Evenly distributes pixel intensities across the entire histogram, improving contrast, especially in concentrated areas.</li>
<li>Adaptive Equalization : Applies histogram equalization in blocks to handle local contrast variations, reducing noise amplification.</li>
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
      <td valign="top"><strong>Image Dst : <em>class</em></strong></td>
    </tr>
  </tbody>
</table>

<h2>Examples</h2>

<p>All these examples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Computer Vision ​library to run it).</p>
