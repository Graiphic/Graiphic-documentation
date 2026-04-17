<h1>AdditiveAttention</h1>

<h2>Description</h2>

<p>Setup and add the additive attention layer into the model during the definition graph step. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="AdditiveAttention" src="assets/AdditiveAttention.png" width="265"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Array_Model.Png" src="assets/input_array_model.png" width="42"/></td>
      <td valign="top"><strong>Models in : <em>array</em></strong>, model architecture. Must be query, value, key (key is optional).</td>
    </tr>
  </tbody>
</table>

<table>
  <tbody>
    <tr>
      <td valign="top" width="75%"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Cluster.Png" src="../../../../_resolved/and/assets/cluster.png" width="42"/></td>
      <td valign="top"><strong>Parameters : </strong>layer parameters.</td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Booleen.Png" src="assets/booleen.png" width="42"/></td>
      <td valign="top"><strong>use scale :</strong> <em><strong>boolean</strong></em>, if True, will create a variable to scale the attention scores.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “True”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Booleen.Png" src="assets/booleen.png" width="42"/></td>
      <td valign="top"><strong>training? :</strong> <em><strong>boolean</strong></em>, whether the layer is in training mode (can store data for backward).</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “True”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Booleen.Png" src="assets/booleen.png" width="42"/></td>
      <td valign="top"><strong>store? :</strong> <em><strong>boolean</strong></em>, whether the layer stores the last iteration gradient (accessible via the “get_gradients” function).</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “False”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Booleen.Png" src="assets/booleen.png" width="42"/></td>
      <td valign="top"><strong>update? :</strong> <em><strong>boolean</strong></em>, whether the layer’s variables should be updated during backward. Equivalent to freeze the layer.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “True”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Array_Double.Png" src="assets/input_array_double.png" width="42"/></td>
      <td valign="top"><strong>lda coeff :</strong> <em><strong>float</strong></em>, defines the coefficient by which the loss derivative will be multiplied before being sent to the previous layer (since during the backward run we go backwards).</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “1”.</td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="25%"><p align="center"><img src="assets/param_attention.png" alt="param_attention" width="79" /></p></td>
    </tr>
  </tbody>
</table>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Array_String.Png" src="assets/input_array_string.png" width="42"/></td>
      <td valign="top"><strong>name (optional) :</strong> <em><strong>string,</strong></em> name of the layer.</td>
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

<p>List of the following tensors:</p>

<ul>
<li>query : Query <em>Tensor</em> of shape [batch_size, Tq, dim].</li>
<li>value : Value <em>Tensor</em> of shape [batch_size, Tv, dim].</li>
<li>key : Optional key <em>Tensor</em> of shape [batch_size, Tv, dim]. If not given, will use <em>value</em> for both <em>key</em> and <em>value</em>, which is the most common case.</li>
</ul>

<h3>Output shape</h3>

<p>Attention outputs of shape [batch_size, Tq, dim].</p>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>

<h3>AdditiveAttention layer with two identical input layer shape</h3>

<p align="center"><img src="assets/1-additiveattention-with-two-identical-input-layer-shape.png" alt="1 - AdditiveAttention with two identical input layer shape" width="260" /></p>

<p>1 – Generate a set of data</p>

<p>We generate two array of data of type single and shape [batch_size = 10, Tq &amp; Tv = 7, dim = 10] (same input shape).</p>

<p>2 – Define graph</p>

<p>We first define two input layers named “query_input” and “value_input”. This layers is setup as an input array shaped [Tq = 7, dim = 10] and [Tv = 7, dim = 10].<br/>Finally, we construct an array of the two graphs generated at the input of AdditiveAttention.</p>

<p>3 – Summarize graph</p>

<p>Returns the summary of the model in file text.</p>

<p>4 – Run graph</p>

<p>We call the forward method and retrieve the result with the “Prediction 3D” method.<br/>This method returns two variables, the first one is the layer information (cluster composed of the layer name, the graph index and the shape of the output layer) and the second one is the prediction with a shape of [batch_size, Tq, dim].</p>

<h3>AdditiveAttention layer with two different input layer shape</h3>

<p align="center"><img src="assets/2-additiveattention-with-two-different-input-layer-shape.png" alt="2 - AdditiveAttention with two different input layer shape" width="260" /></p>

<p>1 – Generate a set of data</p>

<p>We generate two array of data of type single and shape1 [batch_size = 10, Tq = 4, dim = 10] and shape2 [batch_size = 10, Tv = 7, dim = 10] (different input shape).<br/>We can only modify the first dimension (Tq or Tv) because the layer won’t accept different dimension between query, value and key.</p>

<p>2 – Define graph</p>

<p>We first define two input layers named “query_input” and “value_input”. This layers is setup as an input array shaped [Tq = 4, dim = 10] and [Tv = 7, dim = 10].<br/>Finally, we construct an array of the two graphs generated at the input of AdditiveAttention.</p>

<p>3 – Summarize graph</p>

<p>Returns the summary of the model in file text.</p>

<p>4 – Run graph</p>

<p>We call the forward method and retrieve the result with the “Prediction 3D” method.<br/>This method returns two variables, the first one is the layer information (cluster composed of the layer name, the graph index and the shape of the output layer) and the second one is the prediction with a shape of [batch_size, Tq, dim].</p>
