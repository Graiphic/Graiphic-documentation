<h1>algorithm</h1>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Enum.Png" src="assets/enum.png" width="42"/></td>
      <td valign="top"><strong>algorithm :</strong> <em><strong>enum</strong></em>, (name of optimizer) for optimizer instance.</td>
    </tr>
    <tr>
      <td width="64" valign="top"></td>
      <td valign="top">Default value “adam”.</td>
    </tr>
  </tbody>
</table>

<h4>Adadelta</h4>

<p>Adadelta scales the learning rate based on the historical gradient while only taking into account the recent time window and not the entire history, like AdaGrad. Also uses a component that serves as an acceleration term, which accumulates historical updates (similar to momentum).</p>

<table>
  <tbody>
    <tr>
      <td valign="top" width="33%"><p align="center"><img alt="formule" src="assets/formule.PNG" width="220"/></p></td>
      <td valign="top" width="67%"><p><img alt="alpha.PNG" src="assets/alpha.PNG" width="17"/> are accumulated gradients.<br/><img alt="beta1.PNG" src="assets/beta1.PNG" width="25"/> are accumulated updates.<br/><img alt="beta2.PNG" src="assets/beta2.PNG" width="21"/> are a decay constant.<br/><img alt="beta3.PNG" src="assets/beta3.PNG" width="20"/> are gradients.<br/><img alt="biases_momentum1.PNG" src="assets/biases_momentum1.PNG" width="18"/> are learning rate.<br/><img alt="biases_momentum2.PNG" src="assets/biases_momentum2.PNG" width="15"/> are numerical stability (e-7).<br/><img alt="delta_weight.PNG" src="assets/delta_weight.PNG" width="30"/> are rescaled gradients.<br/><img alt="epsilon.PNG" src="assets/epsilon.PNG" width="33"/> are weight.</p></td>
    </tr>
  </tbody>
</table>

<h4>Adagrad</h4>

<p>Adagrad is an optimizer with parameter-specific learning rates, which are adapted relative to how frequently a parameter gets updated during training. The more updates a parameter receives, the smaller the updates.</p>

<table>
  <tbody>
    <tr>
      <td valign="top" width="33%"><p align="center"><img alt="formule" src="assets/formule.PNG" width="220"/></p></td>
      <td valign="top" width="67%"><p><img alt="grad.PNG" src="assets/grad.PNG" width="17"/> are momentum.<br/><img alt="learning_rate.PNG" src="assets/learning_rate.PNG" width="20"/> are gradients of the parameters we want to update.<br/><img alt="momentum1.PNG" src="assets/momentum1.PNG" width="18"/> are learning rate.<br/><img alt="biases_momentum2.PNG" src="assets/biases_momentum2.PNG" width="15"/> are smoothing term (avoids division by zero).<br/><img alt="weight.PNG" src="assets/weight.PNG" width="18"/> are weight.</p></td>
    </tr>
  </tbody>
</table>

<h4>Adam</h4>

<p>Adam optimization is a stochastic gradient descent method that is based on adaptive estimation of first-order and second-order moments.</p>

<table>
  <tbody>
    <tr>
      <td valign="top" width="33%"><p align="center"><img alt="formule" src="assets/formule.PNG" width="220"/></p></td>
      <td valign="top" width="67%"><p><img alt="weight_update.PNG" src="assets/weight_update.PNG" width="25"/> and <img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="17"/> are estimates of the first moment (the mean) and the second moment (the uncentered variance) of the gradients respectively.<br/><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="24"/> and <img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="17"/> are bias-corrected first and second moment estimates.<br/><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="21"/> and <img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="19"/> are momentum coefficient.<br/><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="20"/> are gradients of the parameters we want to update.<br/><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="18"/> are learning rate.<br/><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="15"/> are smoothing term (avoids division by zero).<br/><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="18"/> are weight.</p></td>
    </tr>
  </tbody>
</table>

<h4>Adamax</h4>

<p>AdaMax algorithm is an extension to the Adaptive Movement Estimation (Adam) Optimization algorithm. More broadly, is an extension to the Gradient Descent Optimization algorithm. Adam can be understood as updating weights inversely proportional to the scaled L2 norm (squared) of past gradients. AdaMax extends this to the so-called infinite norm (max) of past gradients.</p>

<table>
  <tbody>
    <tr>
      <td valign="top" width="33%"><p align="center"><img alt="formule" src="assets/formule.PNG" width="220"/></p></td>
      <td valign="top" width="67%"><p><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="25"/> and <img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="17"/> are momentum.<br/><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="21"/> and <img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="19"/> are momentum coefficient.<br/><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="20"/> are gradients of the parameters we want to update.<br/><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="18"/> are learning rate.<br/><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="18"/> are updated learning rate.<br/><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="15"/> are smoothing term (avoids division by zero).<br/><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="18"/> are weight.</p></td>
    </tr>
  </tbody>
</table>

<h4>Inertia</h4>

<table>
  <tbody>
    <tr>
      <td valign="top" width="33%"><p align="center"><img alt="formule" src="assets/formule.PNG" width="220"/></p></td>
      <td valign="top" width="67%"><p><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="17"/> are momentum<br/><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="18"/> are momentum coefficient.<br/><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="20"/> are gradients of the parameters we want to update.<br/><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="18"/> are learning rate.<br/><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="18"/> are weight.</p></td>
    </tr>
  </tbody>
</table>

<h4>NAdam</h4>

<p>Much like Adam is essentially RMSprop with momentum, Nadam is Adam with Nesterov momentum.</p>

<table>
  <tbody>
    <tr>
      <td valign="top" width="33%"><p align="center"><img alt="formule" src="assets/formule.PNG" width="220"/></p></td>
      <td valign="top" width="67%"><p><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="25"/> and <img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="17"/> are estimates of the first moment (the mean) and the second moment (the uncentered variance) of the gradients respectively.<br/><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="24"/> and <img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="17"/> are bias-corrected first and second moment estimates.<br/><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="21"/> and <img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="19"/> are momentum coefficient.<br/><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="20"/> are gradients of the parameters we want to update.<br/><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="18"/> are learning rate.<br/><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="15"/> are smoothing term (avoids division by zero).<br/><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="18"/> are weight.</p></td>
    </tr>
  </tbody>
</table>

<h4>Nesterov</h4>

<p>Nesterov momentum is an extension of momentum that involves calculating the decaying moving average of the gradients of projected positions in the search space rather than the actual positions themselves.</p>

<table>
  <tbody>
    <tr>
      <td valign="top" width="33%"><p align="center"><img alt="formule" src="assets/formule.PNG" width="220"/></p></td>
      <td valign="top" width="67%"><p><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="25"/> are momentum<br/><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="18"/> are momentum coefficient.<br/><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="20"/> are gradients of the parameters we want to update.<br/><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="18"/> are learning rate.<br/><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="18"/> are weight.</p></td>
    </tr>
  </tbody>
</table>

<h4>RMSprop</h4>

<p>The gist of RMSprop is to:</p>

<ol>
<li>Maintain a moving (discounted) average of the square of gradients</li>
<li>Divide the gradient by the root of this average</li>
</ol>

<p>This implementation of RMSprop uses plain momentum, not Nesterov momentum.<br/>The centered version additionally maintains a moving average of the gradients, and uses that average to estimate the variance.</p>

<table>
  <tbody>
    <tr>
      <td valign="top" width="33%"><p align="center"><img alt="formule" src="assets/formule.PNG" width="220"/></p></td>
      <td valign="top" width="67%"><p><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="17"/> are momentum.<br/><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="21"/> are momentum coefficient.<br/><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="20"/> are gradients of the parameters we want to update.<br/><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="18"/> are learning rate.<br/><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="15"/> are smoothing term (avoids division by zero).<br/><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="18"/> are weight.</p></td>
    </tr>
  </tbody>
</table>

<h4>SGD</h4>

<table>
  <tbody>
    <tr>
      <td valign="top" width="33%"><p align="center"><img alt="formule" src="assets/formule.PNG" width="220"/></p></td>
      <td valign="top" width="67%"><p><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="20"/> are gradients of the parameters we want to update.<br/><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="18"/> are learning rate.<br/><img alt="Image Missing.Svg" src="../../../../_assets/image-missing.svg" width="18"/> are weight.</p></td>
    </tr>
  </tbody>
</table>

<p>This parameter is used in <strong>add_to_graph</strong> an <strong>define</strong> VIs of the <strong>AdditiveAttention</strong>, <strong>Attention</strong>, <strong>BatchNormalization</strong>, <strong>Conv1D</strong>, <strong>Conv1DTranspose</strong>, <strong>Conv2D</strong>, <strong>Conv2DTranspose</strong>, <strong>Conv3D</strong>, <strong>Conv3DTranspose</strong>, <strong>Dense</strong>, <strong>DepthwiseConv2D</strong>, <strong>Embedding</strong>, <strong>GRU</strong>, <strong>LayerNormalization</strong>, <strong>LSTM</strong>, <strong>MultiHeadAttention</strong>, <strong>SeparableConv1D</strong>, <strong>SeparableConv2D</strong>, <strong>SimpleRNN</strong>, <strong>PReLU</strong>, <strong>ConvLSTM1DCell</strong>, <strong>ConvLSTM2DCell</strong>, <strong>ConvLSTM3DCell</strong>, <strong>GRUCell</strong>, <strong>LSTMCell</strong>, <strong>SimpleRNNCell</strong> layers.</p>
