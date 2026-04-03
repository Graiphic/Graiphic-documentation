<h1>Set all training status</h1>

<h2>Description</h2>

<p>Sets for all layers contained in the model the state of the boolean “training?”. If the boolean is “True”, then a layer backward is performed.</p>

<p align="center"><img src="assets/set_all_training_status.png" alt="set_all_training_status" width="228" /></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Model.Png" src="assets/input_model.png" width="42"/></td>
      <td valign="top"><strong>Model in : </strong>model architecture.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Booleen.Png" src="assets/booleen.png" width="42"/></td>
      <td valign="top"><strong>training? : <em>boolean</em>,</strong> performs the backward of the layer if true.</td>
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

<h3>Using the “Set All Train Status” function</h3>

<p align="center"><img src="assets/set_all_train_status.png" alt="set_all_train_status" width="260" /></p>

<p>1 – Define Graph</p>

<p>We define the graph with one input and two Dense layers named Dense1 and Dense2 parameterized in different ways.</p>

<p>2 – Set Function</p>

<p>We use the “Set All Train Status” function to set to “True” the boolean that allows the training of a layer(training?). The value of the boolean is applied to all layers of the model.</p>

<p>3 – Get Function</p>

<p>We use the “Get All Train Status” function to get the value of the “training?” parameter for all layers of the model.</p>
