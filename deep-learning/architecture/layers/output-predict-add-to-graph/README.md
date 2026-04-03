<h1>Output Predict</h1>

<h2>Description</h2>

<p>Setup and add the output layer into the model during the definition graph step. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img src="assets/output_predict_add_to_graph.png" alt="Output_Predict_Add_To_Graph.Png" width="228" /></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Out Array Integer 32.Png" src="assets/out-array-integer-32.png" width="42"/></td>
      <td valign="top"><strong>index : <em>integer, </em></strong>position of the output in the graph. This is used only if the <strong>Runtime</strong> → <strong>Output Data VI</strong>.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Array_Enum.Png" src="assets/output_array_enum.png" width="42"/></td>
      <td valign="top"><strong>dtype</strong><strong> :</strong> <em><strong>enum,</strong></em> data type of the input tensor.</td>
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

<h2>Dimension</h2>

<h3>Input shape</h3>

<p>Input tensor (of any rank).</p>

<h3>Output shape</h3>

<p>Same shape as input.</p>
