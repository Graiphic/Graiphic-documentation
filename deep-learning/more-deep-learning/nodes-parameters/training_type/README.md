<h1>type</h1>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Enum.Png" src="assets/enum.png" width="42"/></td>
      <td valign="top"><strong>type : <em>enum, </em></strong>defines how the initializer behaves when the graph is used in training mode. It determines whether the tensor is treated as a constant, as trainable weights, or as frozen weights. During inference, it makes no difference whether the type is <code>Constant</code>, <code>Train Weights</code>, or <code>Frozen Weights</code>.</td>
    </tr>
  </tbody>
</table>

<h4>Constant</h4>

<p>The initializer is treated as a fixed, non-trainable variable (e.g., a constant coefficient in a multiplication).</p>

<h4>Train Weight</h4>

<p>The initializer is treated as trainable weights during training (it will be updated by the optimizer).</p>

<h4>Frozen Weight</h4>

<p>The initializer is treated as weights, but they remain frozen (not updated) during training.</p>
