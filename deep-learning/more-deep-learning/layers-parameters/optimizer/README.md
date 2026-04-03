<h1>optimizer</h1>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Enum.Png" src="assets/enum.png" width="42"/></td>
      <td valign="top"><strong>optimizer :</strong> <em><strong>enum</strong></em>, updates the model’s weights during training based on the computed gradients, guiding the model toward minimizing the loss function.</td>
    </tr>
  </tbody>
</table>

<h4>Default</h4>

<p>By default, the optimizer used is Adam, with the following preset parameters :<br/>learning rate = 0.001, beta1 = 0.9, beta2 = 0.999, weight decay = 0, epsilon = 1e-7, and mode = Pytorch.<br/>These values provide a robust and general-purpose configuration suitable for most deep learning tasks without requiring manual tuning.</p>

<h4>Adam</h4>

<p>The Adam optimizer (Adaptive Moment Estimation) is one of the most widely used algorithms for training neural networks. It combines the benefits of momentum and adaptive learning rates to provide efficient and reliable convergence, especially for large-scale or sparse problems.</p>

<h4>SGD</h4>

<p>The SGD optimizer (Stochastic Gradient Descent) is the simplest and most classical optimization algorithm used in machine learning. It updates model weights by moving in the opposite direction of the gradient of the loss function with respect to the parameters. Although less sophisticated than Adam, it is efficient and predictable when properly tuned.</p>
