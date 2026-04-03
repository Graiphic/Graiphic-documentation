<h1>Set warning parameters</h1>

<h2>Description</h2>

<p>Sets the parameters of warning. If “Display Warning ?” is set to “True” then the warning messages are displayed.</p>

<p align="center"><img src="assets/set_warning_param.png" alt="set_warning_param" width="260" /></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Model.Png" src="assets/input_model.png" width="42"/></td>
      <td valign="top"><strong>Model in : </strong>model architecture.</td>
    </tr>
  </tbody>
</table>

<table>
  <tbody>
    <tr>
      <td valign="top" width="70%"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Cluster.Png" src="assets/cluster.png" width="42"/></td>
      <td valign="top"><strong>Warning Param :</strong> <em><strong>cluster</strong></em></td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Enum.Png" src="assets/enum.png" width="42"/></td>
      <td valign="top"><strong>Language : <em>enum</em>,</strong> warning language.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Booleen.Png" src="assets/booleen.png" width="42"/></td>
      <td valign="top"><strong>Display Warning ? : <em>boolean</em>,</strong> display warning if true.</td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img src="assets/in_warning_param.png" alt="in_warning_param" width="101" /></p></td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Model.Png" src="assets/output_model.png" width="42"/></td>
      <td valign="top"><strong>Model out : </strong>model architecture.</td>
    </tr>
  </tbody>
</table>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>

<h3>Using the “Set Warning Param” function</h3>

<p align="center"><img src="assets/set_warning_params.png" alt="set_warning_params" width="260" /></p>

<p>1 – Set Function</p>

<p>The “Set Warning Param” function is used to define the language of the warnings and if they are displayed.</p>

<p>2 – Define Graph</p>

<p>We define the graph with one input and Dense layers. We also add an input via the “in/out param” input of the Dense layer. Since here two inputs are defined a warning will be issued.</p>

<p>3 – Get Function</p>

<p>We use the “Get Warning Param” function to get the settings made.</p>
