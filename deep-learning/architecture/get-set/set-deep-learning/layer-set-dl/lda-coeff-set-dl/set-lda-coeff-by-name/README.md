<h1>Set “lda_coeff” by name</h1>

<h2>Description</h2>

<p>Sets the loss derivative attenuation coefficient of layer selected by the name given as input.</p>

<p align="center"><img src="assets/set_lda_coeff_by_name.png" alt="set_lda_coeff_by_name" width="228" /></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Model.Png" src="assets/input_model.png" width="42"/></td>
      <td valign="top"><strong>Model in : </strong>model architecture.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="String.Png" src="assets/string.png" width="42"/></td>
      <td valign="top"><strong>name : <em>string</em>, </strong>layer name.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Single.Png" src="assets/single.png" width="42"/></td>
      <td valign="top"><strong>lda_coeff : <em>float, </em></strong>loss derivative attenuation coefficient value.</td>
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

<h3>Using the “Set lda_coeff by name” function</h3>

<p align="center"><img src="assets/set_lda_coef_by_name.png" alt="set_lda_coef_by_name" width="260" /></p>

<p>1 – Define Graph</p>

<p>We define the graph with one input and two Dense layers named Dense1 and Dense2. We set the Dense1 layer with a “lda_coeff” equal to 2 and the Dense2 layer with a “lda_coeff” equal to 5.</p>

<p>2 – Get Function</p>

<p>We use the “Set lda_coeff by index” function to set the loss derivative attenuation of the layer named Dense2 with the value 1.</p>

<p>2 – Get Function</p>

<p>We use the “Get All lda_coeff” function to get the value of this parameter for all layers in the model.</p>
