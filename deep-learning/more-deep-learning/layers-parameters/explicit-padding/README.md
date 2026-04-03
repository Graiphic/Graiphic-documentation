<h1>explicit padding</h1>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Array Integer 32.Png" src="assets/array-integer-32.png" width="42"/></td>
      <td valign="top"><strong>explicit padding : <em>array</em></strong>, specifies the number of pixels to pad at the beginning and end of each spatial axis. Batch and channel axes are not padded. Only used when padding = <strong>EXPLICIT</strong>.</td>
    </tr>
  </tbody>
</table>

<p>Format</p>

<p>[x1_begin, x2_begin, …, x1_end, x2_end, …]<br/>Where xi_begin and xi_end are the number of pixels added before and after spatial dimension i.</p>

<p>Examples</p>

<p>if 3D input (shape: N x C x H)<br/>Padding 1 pixel at the beginning and 2 at the end of the height axis : explicit_padding = [1, 2]</p>

<p>if 4D input (shape: N x C x H x W)<br/>Padding 1 at the beginning and 2 at the end of height, and 3 at the beginning and 4 at the end of width : explicit_padding = [1, 3, 2, 4]</p>

<p>if 5D input (shape: N x C x D x H x W)<br/>Padding 1 at the beginning and 2 at the end of depth, 3/4 for height, and 5/6 for width : explicit_padding = [1, 3, 5, 2, 4, 6]<br/>The length of explicit_padding must always be 2 × number of spatial dimensions.</p>
