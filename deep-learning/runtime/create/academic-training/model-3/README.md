<h1>Create Academic Training Session From Model</h1>

<h3>Description</h3>

<p>Initialize an Academic Training Session from a DeepLearning Toolkit Model. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="create_academic_model.png" src="assets/create_academic_model.png" width="364"/></p>

<h3>Input parameters</h3>

<p><img alt="Enum.Png" src="assets/enum.png" width="32"/><strong>Execution Device : <em>enum</em>, </strong>selects the hardware device on which the model will run.<br/><img alt="Input_Model.Png" src="assets/input_model.png" width="32"/><strong>Model in : <em>object</em>, </strong>model architecture.</p>

<table>
  <tbody>
    <tr>
      <td valign="top" width="70%"><p><img alt="Cluster.Png" src="assets/cluster.png" width="32"/><strong>Parameters : <em>cluster,</em></strong></p>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Single.Png" src="assets/single.png" width="42"/></td>
      <td valign="top"><strong>max_norm : <em>float, </em></strong>maximum global gradient norm (enables clipping if > 0).</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Enum.Png" src="assets/enum.png" width="42"/></td>
      <td valign="top"><strong>norm_type : <em>enum, </em></strong>type of norm used to compute <code>grad_norm</code> (commonly 1 = L1, 2 = L2).</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Booleen.Png" src="assets/booleen.png" width="42"/></td>
      <td valign="top"><strong> display_norm : <em>boolean, </em></strong>adds <code>grad_norm</code> as a model output if set to 1.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Booleen.Png" src="assets/booleen.png" width="42"/></td>
      <td valign="top"><strong> independent_loss_model : <em>boolean, </em></strong>if true, splits the model into 3 stages (forward, loss, backward) instead of 2 (forward+loss, backward).</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Enum.Png" src="assets/enum.png" width="42"/></td>
      <td valign="top"><strong>checkpoint generation : <em>enum</em>, </strong>defines what is saved in the checkpoint: <code>"Weight"</code> (weights only) or <code>"Weight + Momentum"</code> (weights and optimizer momentums). Momentums must already be set in the <code>"Model in"</code>.</td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img alt="param_create_academic_model" src="assets/param_create_academic_model.png" width="220"/></p></td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Academic.Png" src="assets/output_academic.png" width="42"/></td>
      <td valign="top"><strong>Academic Training out</strong> <strong>: <em>object, </em></strong>academic training session.</td>
    </tr>
  </tbody>
</table>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>
