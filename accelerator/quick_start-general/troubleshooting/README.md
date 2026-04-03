<h1>Troubleshooting</h1>

<p>This section presents the different errors that can appear when using the library.</p>

<table>
  <thead>
    <tr>
      <th><strong>Code</strong></th>
      <th><strong>VI</strong></th>
      <th><strong>Information</strong></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>5001</td>
      <td>check_bidirectional_output</td>
      <td>The layers sent in the &#8220;layer&#8221; and &#8220;backward_layer&#8221; parameters of the <a href="/deep-learning/architecture/layers/bidirectional-add-to-graph/README.md">Bidirectional</a> layer must have the same output shape, unless the value of the merge_mode parameter is &#8220;concat&#8221;. For layers to have the same output shape, the same value must be set in the &#8220;units&#8221; parameter (parameter of the layer sent to the bidirectional layer).</td>
    </tr>
    <tr>
      <td>5002</td>
      <td>check_bidirectional_return_sequences</td>
      <td>The layers sent in the &#8220;layer&#8221; and &#8220;backward_layer&#8221; parameters of the <a href="/deep-learning/architecture/layers/bidirectional-add-to-graph/README.md">Bidirectional</a> layer must have the same value for the return_sequences parameter.</td>
    </tr>
    <tr>
      <td>5003</td>
      <td>check_conv</td>
      <td>The convolution is not feasible because the shape of the input is not large enough.<br> You have three solutions: <ul>
  <li>Enlarge the input size</li>
  <li>Reduce the size of the kernel</li>
  <li>Set the &#8220;padding&#8221; parameter of the layer to &#8220;same&#8221; (padding will be added in such a way as to convolve in all cases)</li>

</ul></td>
    </tr>
    <tr>
      <td>5004 &#8211; 5026 &#8211; 5027</td>
      <td>check_attention</td>
      <td>The entries in the <a href="/deep-learning/architecture/layers/attention-add-to-graph/README.md">Attention</a> layer do not have the correct input shape.</td>
    </tr>
    <tr>
      <td>5004 &#8211; 5005 &#8211; 5026</td>
      <td>check_additive_attention</td>
      <td>The entries in the <a href="/deep-learning/architecture/layers/additive-attention-add-to-graph/README.md">AdditiveAttention</a> layer do not have the correct input shape.</td>
    </tr>
    <tr>
      <td>5004 &#8211; 5026</td>
      <td>check_multiheadattention</td>
      <td>The entries in the <a href="/deep-learning/architecture/layers/multi-head-attention-add-to-graph/README.md">MultiHeadAttention</a> layer do not have the correct input shape.</td>
    </tr>
    <tr>
      <td>5006</td>
      <td>check_input_same_index</td>
      <td>The index selected when formatting the data at the input of the forward is already defined.</td>
    </tr>
    <tr>
      <td>5007</td>
      <td>check_input_shape</td>
      <td>The input layer does not exist. Add the <a href="/deep-learning/architecture/layers/input-add-to-graph/README.md">Input</a> layer at the beginning of the model or use the &#8220;in/out param&#8221; parameter of the layer that starts your model.</td>
    </tr>
    <tr>
      <td>5008</td>
      <td>check_nb_input</td>
      <td>The number of inputs sent to the forward does not match the number of inputs in the model.</td>
    </tr>
    <tr>
      <td>5009</td>
      <td>check_nb_y_true</td>
      <td>The number of outputs (y_true) sent to the loss does not correspond to the number of trainable outputs of the model.<br> Caution : if your forward is in training mode it will not allow loss, if you want metric loss, use metric functionalities.</td>
    </tr>
    <tr>
      <td>5010</td>
      <td>warning_input_shape</td>
      <td>An input already exists, so the input shape you defined in the &#8220;in/out param&#8221; parameter is not taken into account.</td>
    </tr>
    <tr>
      <td>5011</td>
      <td>check_output_same_index</td>
      <td>The index selected when formatting the data sent to the loss (y_true) is already defined.</td>
    </tr>
    <tr>
      <td>5012</td>
      <td>check_shape</td>
      <td>The inputs of the operand (<a href="/deep-learning/architecture/layers/add-add-to-graph/README.md">Add</a> or <a href="/deep-learning/architecture/layers/average-add-to-graph/README.md">Average</a> or <a href="/deep-learning/architecture/layers/multiply-add-to-graph/README.md">Multiply</a> or <a href="/deep-learning/architecture/layers/substract-add-to-graph/README.md">Substract</a>) do not have the same shape.</td>
    </tr>
    <tr>
      <td>5013</td>
      <td>check_shape_concat</td>
      <td>The entries of the <a href="/deep-learning/architecture/layers/concatenate-add-to-graph/README.md">Concatenate</a> layer do not have the same shape. Note that the size of the axis on which we concatenate can be different. Example: if we have an entry with shape (10, 2, 3), another with shape (10, 2, 4) and the parameter &#8220;axis&#8221; of the layer is 1, then the error occurs because when checking the shape, the layer considers that one entry has a shape of (10, 3) and the other one (10, 4). If &#8220;axis&#8221; is 2, then there is no error because during the verification of the shape, the layer considers that the entries have a shape of (10, 2).</td>
    </tr>
    <tr>
      <td>5014</td>
      <td>check_shape_set_input</td>
      <td>The dimensions of the input array provided does not correspond to those expected.</td>
    </tr>
    <tr>
      <td>5015</td>
      <td>check_shape_set_weight</td>
      <td>The dimensions of the weight array provided does not correspond to those expected.</td>
    </tr>
    <tr>
      <td>5016</td>
      <td>check_shape_y_true</td>
      <td>The dimensions of the y_true array provided does not correspond to those expected.</td>
    </tr>
    <tr>
      <td>5018</td>
      <td>warning_output_index</td>
      <td>The output order specified is out of bound (x &lt; 0 or x &gt; nb_output).</td>
    </tr>
    <tr>
      <td>5019</td>
      <td>warning_input_name</td>
      <td>The layer name specified isn&#8217;t an input of model.</td>
    </tr>
    <tr>
      <td>5020</td>
      <td>check_output_same_name</td>
      <td>The name specified when formatting the data sent to the loss (y_true) is already defined.</td>
    </tr>
    <tr>
      <td>5021</td>
      <td>warning_input_index</td>
      <td>The input order specified is out of bound (x &lt; 0 or x &gt; nb_input).</td>
    </tr>
    <tr>
      <td>5022</td>
      <td>display_name_error</td>
      <td>The name specified doesn&#8217;t exist in the graph.</td>
    </tr>
    <tr>
      <td>5023 &#8211; 5039</td>
      <td>check_gpu_layer</td>
      <td>One or more layers are not available in CUDA version.</td>
    </tr>
    <tr>
      <td>5024</td>
      <td>display_dim_error</td>
      <td>The layer does not support the given dimension.</td>
    </tr>
    <tr>
      <td>5028</td>
      <td>check_dim</td>
      <td>The input is incompatible with the layer.</td>
    </tr>
    <tr>
      <td>5029</td>
      <td>check_dim</td>
      <td>The product of the input form is not equal to the product of the output form. Example: for an input shape (10, 2, 3, 5) the product is equal to 300 (10 * 2 * 3 * 5) then, in output if we want 3D we will have for example a shape of (10, 3, 10).</td>
    </tr>
    <tr>
      <td>5030</td>
      <td>check_graphs_shape</td>
      <td>The output shape of the first graph is incompatible with the input shape of the second.</td>
    </tr>
    <tr>
      <td>5031</td>
      <td>warning_y_true_name</td>
      <td>The name shown is not a driveable output of the model.</td>
    </tr>
    <tr>
      <td>5032 &#8211; 5033</td>
      <td>check_pool_shape</td>
      <td>The kernel size or the stride does not have the right shape or right values.</td>
    </tr>
    <tr>
      <td>5034</td>
      <td>check_filter_units</td>
      <td>The value assigned to the &#8220;n_filters&#8221; parameter must be strictly positive.</td>
    </tr>
    <tr>
      <td>5035</td>
      <td>check_embedding_input_output_dim</td>
      <td>The <a href="/deep-learning/architecture/layers/embedding-add-to-graph/README.md">Embedding</a> layer must have strictly positive the &#8220;input_dim&#8221; and &#8220;output_dim&#8221; parameters value.</td>
    </tr>
    <tr>
      <td>5036</td>
      <td>check_rnn_gpu_integration</td>
      <td>The &#8220;activation&#8221; parameter(s) of the cells sent to the RNN layer is not compatible with the CuDNN version.</td>
    </tr>
    <tr>
      <td>5037</td>
      <td>check_fit_metric_best</td>
      <td>The metric selected in the &#8220;Comparison Metric&#8221; parameter of the &#8220;Fit&#8221; function is not in the &#8216;metrics_array&#8217;.</td>
    </tr>
    <tr>
      <td>5038</td>
      <td>check_multi_input_batch</td>
      <td>The batch size is not the same for every inputs of operand layer (<a href="/deep-learning/architecture/layers/add-add-to-graph/README.md">Add</a> or <a href="/deep-learning/architecture/layers/average-add-to-graph/README.md">Average</a> or <a href="/deep-learning/architecture/layers/multiply-add-to-graph/README.md">Multiply</a> or <a href="/deep-learning/architecture/layers/substract-add-to-graph/README.md">Substract</a>).</td>
    </tr>
    <tr>
      <td>5040 &#8211; 5042</td>
      <td>check_gpu_ready</td>
      <td>Your gpu is not ready. You must have a CUDA compatible graphics card or install CUDA. You can use our <a href="/deep-learning/installation-guide/execution-providers/cuda/README.md">installer</a> to start the installation.</td>
    </tr>
    <tr>
      <td>5043</td>
      <td>warning_attention_scale</td>
      <td>The AdditiveAttention layer has no weight because &#8220;use_scale&#8221; == False.</td>
    </tr>
    <tr>
      <td>5044</td>
      <td>check_index</td>
      <td>The index specified doesn&#8217;t exist in the graph.</td>
    </tr>
    <tr>
      <td>5050</td>
      <td>Licence not installed</td>
      <td>The licence is not installed so toolkit could not run.</td>
    </tr>
    <tr>
      <td>5051</td>
      <td>Licence expired</td>
      <td>Licence expired so toolkit could not run.</td>
    </tr>
    <tr>
      <td>5052</td>
      <td>Runtime Error</td>
      <td>Their is a Runtime error so could not run</td>
    </tr>
    <tr>
      <td>5053</td>
      <td>Reactivation needed</td>
      <td>Licence Reactivation needed (Use SOTA to reactivate the licence on the computer)</td>
    </tr>
  </tbody>
</table>
