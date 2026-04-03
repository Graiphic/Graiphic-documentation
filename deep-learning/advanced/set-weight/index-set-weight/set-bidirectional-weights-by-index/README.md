<h1>Bidirectional</h1>

<h2>Description</h2>

<p>Defines the weights of the Bidirectional layer selected by the index. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img src="assets/set_weights_bidirectional_index.png" alt="Set_Weights_Bidirectional_Index.Png" width="261" /></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Model.Png" src="assets/input_model.png" width="42"/></td>
      <td valign="top"><strong>Model in : </strong>model architecture.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Integer 32.Png" src="assets/integer-32.png" width="42"/></td>
      <td valign="top"><strong>index : <em>integer</em>, </strong>index of layer.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Var In.Png" src="assets/var-in.png" width="42"/></td>
      <td valign="top"><strong>layer : <em>variant, </em></strong>cluster from “<a href="../../../get-weight/index/get-gru-weights-by-index/README.md">gru_weights</a>” or “<a href="../../../get-weight/index/get-lstm-weights-by-index/README.md">lstm_weights</a>” or “<a href="../../../get-weight/index/get-simple-rnn-weights-by-index/README.md">simplernn_weights</a>“.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Var In.Png" src="assets/var-in.png" width="42"/></td>
      <td valign="top"><strong>backward_layer : <em>variant, </em></strong>cluster from “<a href="../../../get-weight/index/get-gru-weights-by-index/README.md">gru_weights</a>” or “<a href="../../../get-weight/index/get-lstm-weights-by-index/README.md">lstm_weights</a>” or “<a href="../../../get-weight/index/get-simple-rnn-weights-by-index/README.md">simplernn_weights</a>“.</td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Model.Png" src="assets/output_model.png" width="42"/></td>
      <td valign="top"><strong>Model out : </strong>model architecture.</td>
    </tr>
  </tbody>
</table>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>
