<h1>NegativeLogLikelihoodLoss</h1>

<h2>Description</h2>

<p>A NegativeLogLikelihoodLoss operator computes (weighted) negative log likelihood loss.</p>

<p align="center"><img alt="node_negative_log_likelihood_loss.png" src="assets/node_negative_log_likelihood_loss.png" width="299"/></p>

<p>Its “input” tensor has the shape of (N, C, d1, d2, …, dk) where k &gt;= 0. The “input” tensor contains log-probabilities for input[n, :, d_1, d_2,…, d_k] being in a class of [0, C). The operator’s “target” input tensor has the shape of (N, d1, d2, …, dk). It encodes class labels (one of C classes) or it may contain a special value (indicated by an attribute ignore_index) for N x d1 x d2 x … x dk samples. The loss value for input[n, :, d_1, d_2,…d_k] being classified as class c = target[n][d_1][d_2]…[d_k] is computed as : loss[n][d_1][d_2]…[d_k] = –input[n][c][d_1][d_2]…[d_k].</p>

<p>When an optional “weight” is provided, the sample loss is calculated as : loss[n][d_1][d_2]…[d_k] = –input[n][c][d_1][d_2]…[d_k] * weight[c].</p>

<p>loss is zero for the case when target-value equals ignore_index.</p>

<p>loss</p>

<p>[</p>

<p>n</p>

<p>][</p>

<p>d_1</p>

<p>][</p>

<p>d_2</p>

<p>]</p>

<p>...</p>

<p>[</p>

<p>d_k</p>

<p>]</p>

<p>=</p>

<p>0</p>

<p>,</p>

<p>when</p>

<p>target</p>

<p>[</p>

<p>n</p>

<p>][</p>

<p>d_1</p>

<p>][</p>

<p>d_2</p>

<p>]</p>

<p>...</p>

<p>[</p>

<p>d_k</p>

<p>]</p>

<p>=</p>

<p>ignore_index</p>

<p>If “reduction” attribute is set to “none”, the operator’s output will be the above loss with shape (N, d1, d2, …, dk). If “reduction” attribute is set to “mean” (the default attribute value), the output loss is (weight) averaged : mean(loss), if “weight” is not provided,</p>

<p>or if weight is provided, sum(loss) / sum(weight[target[n][d_1][d_2]…[d_k]]]), for all samples.</p>

<p>If “reduction” attribute is set to “sum”, the output is a scalar: <code>sum(loss)</code>.</p>

<p>See also <a href="https://pytorch.org/docs/stable/nn.html#torch.nn.NLLLoss">https://pytorch.org/docs/stable/nn.html#torch.nn.NLLLoss</a>.</p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Array_String.Png" src="assets/input_array_string.png" width="42"/></td>
      <td valign="top"><strong><a href="../../../../../../more-deep-learning/nodes-parameters/specified_outputs_name/README.md">specified_outputs_name</a> : <em>array, </em></strong>this parameter lets you manually assign custom names to the output tensors of a node.</td>
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
      <td valign="top"><strong>Graphs in :</strong> <strong><em>cluster,</em></strong> ONNX model architecture.</td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Object_3.Png" src="assets/input_object_3.png" width="42"/></td>
      <td valign="top"><strong>input (heterogeneous) – T</strong> <strong>:</strong> <em><strong>object,</strong></em> input tensor of shape (N, C) or (N, C, d1, d2, …, dk).</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Object_3.Png" src="assets/input_object_3.png" width="42"/></td>
      <td valign="top"><strong>target (heterogeneous) – Tind : <em>object, </em></strong>target tensor of shape (N) or (N, d1, d2, …, dk). Target element value shall be in range of [0, C). If ignore_index is specified, it may have a value outside [0, C) and the target values should either be in the range [0, C) or have the value ignore_index.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Object_3.Png" src="assets/input_object_3.png" width="42"/></td>
      <td valign="top"><strong>weight (optional, heterogeneous) – T : <em>object, </em></strong>optional rescaling weight tensor. If given, it has to be a tensor of size C. Otherwise, it is treated as if having all ones.</td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img alt="input_node_negative_log_likelihood_loss" src="assets/input_node_negative_log_likelihood_loss.png" width="220"/></p></td>
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
      <td valign="top"><strong>Parameters : <em>cluster,</em></strong></td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Integer 32.Png" src="assets/integer-32.png" width="42"/></td>
      <td valign="top"><strong>ignore_index :</strong> <em><strong>integer</strong><strong>,</strong></em> specifies a target value that is ignored and does not contribute to the input gradient. It’s an optional value.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “0”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Enum.Png" src="assets/enum.png" width="42"/></td>
      <td valign="top"><strong>reduction : <em>enum, </em></strong>type of reduction to apply to loss: none, sum, mean (default). ‘none’: the output is the loss for each sample. ‘sum’: the output will be summed. ‘mean’: the sum of the output will be divided by the sum of applied weights.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “mean”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Booleen.Png" src="assets/booleen.png" width="42"/></td>
      <td valign="top"><strong>training? :</strong> <em><strong>boolean</strong><strong>,</strong></em> whether the layer is in training mode (can store data for backward).</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “True”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Double.Png" src="assets/double.png" width="42"/></td>
      <td valign="top"><strong>lda coeff :</strong> <em><strong>float</strong><strong>,</strong></em> defines the coefficient by which the loss derivative will be multiplied before being sent to the previous layer (since during the backward run we go backwards).</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “1”.</td>
    </tr>
  </tbody>
</table></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="String.Png" src="assets/string.png" width="42"/></td>
      <td valign="top"><strong>name (optional) :</strong> <em><strong>string,</strong></em> name of the node.</td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img alt="param_node_negative_log_likelihood_loss" src="assets/param_node_negative_log_likelihood_loss.png" width="220"/></p></td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Object_3.Png" src="assets/output_object_3.png" width="42"/></td>
      <td valign="top"><strong>loss (heterogeneous) – T :</strong> <em><strong>object,</strong></em> the negative log likelihood loss.</td>
    </tr>
  </tbody>
</table>

<h2>Type Constraints</h2>

<p><strong>T</strong> in (<code>tensor(double)</code>, <code>tensor(float)</code>, <code>tensor(float16)</code>) : Constrain input, weight, and output types to floating-point tensors.</p>

<p><strong>Tind</strong> in (<code>tensor(int32)</code>, <code>tensor(int64)</code>) : Constrain target to integer types.</p>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>
