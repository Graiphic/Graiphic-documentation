<h1>Bidirectional</h1>

<h2>Description</h2>

<p>Adds the weights of the Bidirectional layer to the weights table. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="Bidirectional" src="assets/Bidirectional.png" width="275"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td valign="top" width="70%"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Cluster Array In.Png" src="assets/cluster-array-in.png" width="42"/></td>
      <td valign="top"><strong>Weights in : array</strong></td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Integer 32.Png" src="assets/integer-32.png" width="42"/></td>
      <td valign="top"><strong>index : <em>integer,</em></strong> index of layer.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="var-in.png" src="assets/var-in.png" width="42"/></td>
      <td valign="top"><strong>weights : <em>variant,</em></strong> weights values.</td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img alt="weights_in_by_index" src="assets/weights_in_by_index.png" width="220"/></p></td>
    </tr>
  </tbody>
</table>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Integer 32.Png" src="assets/integer-32.png" width="42"/></td>
      <td valign="top"><strong>index : <em>integer</em>, </strong>index of layer.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="var-out.png" src="assets/var-out.png" width="42"/></td>
      <td valign="top"><strong>layer : <em>variant, </em></strong>cluster from “<a href="../../../get-weight/index/get-gru-weights-by-index/README.md">gru_weights</a>” or “<a href="../../../get-weight/index/get-lstm-weights-by-index/README.md">lstm_weights</a>” or “<a href="../../../get-weight/index/get-simple-rnn-weights-by-index/README.md">simplernn_weights</a>“.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Image Missing.Svg" src="../../../../../_assets/image-missing.svg" width="42"/></td>
      <td valign="top"><strong>backward_layer : <em>variant, </em></strong>cluster from “<a href="../../../get-weight/index/get-gru-weights-by-index/README.md">gru_weights</a>” or “<a href="../../../get-weight/index/get-lstm-weights-by-index/README.md">lstm_weights</a>” or “<a href="../../../get-weight/index/get-simple-rnn-weights-by-index/README.md">simplernn_weights</a>“.</td>
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
      <td width="64" valign="top"><img alt="Cluster Array Out.Png" src="assets/cluster-array-out.png" width="42"/></td>
      <td valign="top"><strong>Weights out : array</strong></td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Integer 32 Out.Png" src="assets/integer-32-out.png" width="42"/></td>
      <td valign="top"><strong>index : <em>integer,</em></strong> index of layer.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Image Missing.Svg" src="../../../../../_assets/image-missing.svg" width="42"/></td>
      <td valign="top"><strong>weights : <em>variant,</em></strong> weights values.</td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img alt="weights_out_by_index" src="assets/weights_out_by_index.png" width="220"/></p></td>
    </tr>
  </tbody>
</table>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>
