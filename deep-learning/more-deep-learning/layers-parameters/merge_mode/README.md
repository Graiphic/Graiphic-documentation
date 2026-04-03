<h1>merge_mode</h1>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Enum.Png" src="assets/enum.png" width="42"/></td>
      <td valign="top"><strong>merge_mode : <em>enum</em></strong><em>,</em> mode by which outputs of the forward and backward RNNs will be combined.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “concat”.
<ul>
<li><strong>sum : </strong>Add the tables</li>
<li><strong>mul : </strong>Multiply the tables</li>
<li><strong>concat : </strong>Concatenate the tables</li>
<li><strong>ave : </strong>Averages the tables</li>
</ul></td>
    </tr>
  </tbody>
</table>

<p>This parameter is used in <strong>add_to_graph </strong>and<strong> define</strong> VIs of <strong>Bidirectional</strong> layer.</p>
