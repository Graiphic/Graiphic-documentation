<h1>SoftmaxCrossEntropyLoss</h1>

<h2>Description</h2>

<p>Loss function that measures the softmax cross entropy between ‘scores’ and ‘labels’. This operator first computes a loss tensor whose shape is identical to the labels input.</p>

<p align="center"><img alt="SoftmaxCrossEntropyLoss" src="assets/SoftmaxCrossEntropyLoss.png" width="311"/></p>

<p>If the input is 2-D with shape (N, C), the loss tensor may be a N-element vector L = (l_1, l_2, …, l_N). If the input is N-D tensor with shape (N, C, D1, D2, …, Dk), the loss tensor L may have (N, D1, D2, …, Dk) as its shape and L[j_1][j_2]…[j_k] denotes a scalar element in L. After L is available, this operator can optionally do a reduction operator.</p>

<ul>
<li>shape(scores): (N, C) where C is the number of classes, or (N, C, D1, D2,…, Dk), with K &gt;= 1 in case of K-dimensional loss.</li>
<li>shape(labels): (N) where each value is 0 &lt;= labels &lt;= C-1, or (N, D1, D2,…, Dk), with K &gt;= 1 in case of K-dimensional loss.</li>
</ul>

<p>The loss for one sample, l_i, can calculated as follows:</p>

<p>l</p>

<p>[</p>

<p>i</p>

<p>][</p>

<p>d1</p>

<p>][</p>

<p>d2</p>

<p>]</p>

<p>...</p>

<p>[</p>

<p>dk</p>

<p>]</p>

<p>=</p>

<p>-</p>

<p>y</p>

<p>[</p>

<p>i</p>

<p>][</p>

<p>c</p>

<p>][</p>

<p>d1</p>

<p>][</p>

<p>d2</p>

<p>]</p>

<p>..</p>

<p>[</p>

<p>dk</p>

<p>],</p>

<p>where</p>

<p>i</p>

<p>is</p>

<p>the</p>

<p>index</p>

<p>of</p>

<p>classes</p>

<p>.</p>

<p>or</p>

<p>l</p>

<p>[</p>

<p>i</p>

<p>][</p>

<p>d1</p>

<p>][</p>

<p>d2</p>

<p>]</p>

<p>...</p>

<p>[</p>

<p>dk</p>

<p>]</p>

<p>=</p>

<p>-</p>

<p>y</p>

<p>[</p>

<p>i</p>

<p>][</p>

<p>c</p>

<p>][</p>

<p>d1</p>

<p>][</p>

<p>d2</p>

<p>]</p>

<p>..</p>

<p>[</p>

<p>dk</p>

<p>]</p>

<p>*</p>

<p>weights</p>

<p>[</p>

<p>c</p>

<p>],</p>

<p>if</p>

<p>&#x27;weights&#x27;</p>

<p>is</p>

<p>provided</p>

<p>.</p>

<p>loss is zero for the case when label-value equals ignore_index.</p>

<p>l</p>

<p>[</p>

<p>i</p>

<p>][</p>

<p>d1</p>

<p>][</p>

<p>d2</p>

<p>]</p>

<p>...</p>

<p>[</p>

<p>dk</p>

<p>]</p>

<p>=</p>

<p>0</p>

<p>,</p>

<p>when</p>

<p>labels</p>

<p>[</p>

<p>n</p>

<p>][</p>

<p>d1</p>

<p>][</p>

<p>d2</p>

<p>]</p>

<p>...</p>

<p>[</p>

<p>dk</p>

<p>]</p>

<p>=</p>

<p>ignore_index</p>

<p>where:</p>

<p>p</p>

<p>=</p>

<p>Softmax</p>

<p>(</p>

<p>scores</p>

<p>)</p>

<p>y</p>

<p>=</p>

<p>Log</p>

<p>(</p>

<p>p</p>

<p>)</p>

<p>c</p>

<p>=</p>

<p>labels</p>

<p>[</p>

<p>i</p>

<p>][</p>

<p>d1</p>

<p>][</p>

<p>d2</p>

<p>]</p>

<p>...</p>

<p>[</p>

<p>dk</p>

<p>]</p>

<p>Finally, L is optionally reduced:</p>

<ul>
<li>If reduction = ‘none’, the output is L with shape (N, D1, D2, …, Dk).</li>
<li>If reduction = ‘sum’, the output is scalar: Sum(L).</li>
<li>If reduction = ‘mean’, the output is scalar: ReduceMean(L), or if weight is provided: <code>ReduceSum(L) / ReduceSum(W)</code>, where tensor W is of shape <code>(N, D1, D2, ..., Dk)</code> and <code>W[n][d1][d2]...[dk] = weights[labels[d1][d2]...[dk]]</code>.</li>
</ul>

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
      <td valign="top"><strong>scores (heterogeneous) – T : <em>object, </em></strong>the predicted outputs with shape [batch_size, class_size], or [batch_size, class_size, D1, D2 , …, Dk], where K is the number of dimensions.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Object_3.Png" src="assets/input_object_3.png" width="42"/></td>
      <td valign="top"><strong>labels (heterogeneous) – Tind : <em>object, </em></strong>the ground truth output tensor, with shape [batch_size], or [batch_size, D1, D2, …, Dk], where K is the number of dimensions. Labels element value shall be in range of [0, C). If ignore_index is specified, it may have a value outside [0, C) and the label values should either be in the range [0, C) or have the value ignore_index.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Object_3.Png" src="assets/input_object_3.png" width="42"/></td>
      <td valign="top"><strong>weights (optional, heterogeneous) – T : <em>object, </em></strong>a manual rescaling weight given to each class. If given, it has to be a 1D Tensor assigning weight to each of the classes. Otherwise, it is treated as if having all ones.</td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img alt="input_node_softmax_cross_entropy_loss" src="assets/input_node_softmax_cross_entropy_loss.png" width="220"/></p></td>
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
      <td valign="top"><strong>Parameters : <em>cluster,</em></strong></td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Integer 32.Png" src="assets/integer-32.png" width="42"/></td>
      <td valign="top"><strong>ignore_index : <em>integer,</em></strong> specifies a target value that is ignored and does not contribute to the input gradient. It’s an optional value.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “0”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Enum.Png" src="assets/enum.png" width="42"/></td>
      <td valign="top"><strong>reduction : <em>enum,</em></strong> type of reduction to apply to loss: none, sum, mean(default). ‘none’: no reduction will be applied, ‘sum’: the output will be summed. ‘mean’: the sum of the output will be divided by the number of elements in the output.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “mean”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Booleen.Png" src="assets/booleen.png" width="42"/></td>
      <td valign="top"><strong>training? :</strong> <em><strong>boolean</strong></em>, whether the layer is in training mode (can store data for backward).</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “True”.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Double.Png" src="assets/double.png" width="42"/></td>
      <td valign="top"><strong>lda coeff :</strong> <em><strong>float</strong></em>, defines the coefficient by which the loss derivative will be multiplied before being sent to the previous layer (since during the backward run we go backwards).</td>
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
      <td valign="top"><strong>name (optional) :</strong> <em><strong>string,</strong></em> name of the node.</td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img alt="param__node_softmax_cross_entropy_loss" src="assets/param__node_softmax_cross_entropy_loss.png" width="220"/></p></td>
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
      <td width="64" valign="top"><img alt="Cluster Out.Png" src="assets/cluster-out.png" width="42"/></td>
      <td valign="top"><strong>Graphs out :</strong> <strong><em>cluster,</em></strong> ONNX model architecture.</td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Object_3.Png" src="assets/output_object_3.png" width="42"/></td>
      <td valign="top"><strong>output (heterogeneous) – T : <em>object, </em></strong>weighted loss float Tensor. If reduction is ‘none’, this has the shape of [batch_size], or [batch_size, D1, D2, …, Dk] in case of K-dimensional loss. Otherwise, it is a scalar.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_Object_3.Png" src="assets/output_object_3.png" width="42"/></td>
      <td valign="top"><strong>log_prob (optional, heterogeneous) – T : <em>object, </em></strong>log probability tensor. If the output of softmax is prob, its value is log(prob).</td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img alt="output_node_softmax_cross_entropy_loss" src="assets/output_node_softmax_cross_entropy_loss.png" width="220"/></p></td>
    </tr>
  </tbody>
</table>

<h2>Type Constraints</h2>

<p><strong>T</strong> in (<code>tensor(bfloat16)</code>, <code>tensor(double)</code>, <code>tensor(float)</code>, <code>tensor(float16)</code>) : Constrain input and output types to float tensors.</p>

<p><strong>Tind</strong> in (<code>tensor(int32)</code>, <code>tensor(int64)</code>) : Constrain target to integer types</p>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>
