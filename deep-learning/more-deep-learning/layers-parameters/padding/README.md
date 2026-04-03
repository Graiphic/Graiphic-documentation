<h1>padding</h1>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Enum.Png" src="assets/enum.png" width="42"/></td>
      <td valign="top"><strong>padding : <em>enum,</em></strong> type of padding to apply.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “VALID”.
<ul>
<li><strong>EXPLICIT</strong> : Padding is manually defined through the explicit_padding parameter.</li>
<li><strong>SAME_UPPER</strong> : Pads the input so that output_shape = ceil(input_shape / strides). If the padding is odd, the extra pixel is added at the end.</li>
<li><strong>SAME_LOWER</strong> : Same behavior as ‘SAME_UPPER’, but the extra pixel is added at the beginning.</li>
<li><strong>VALID</strong> : No padding is applied. The operation only uses the fully covered regions of the input.</li>
</ul></td>
    </tr>
  </tbody>
</table>
