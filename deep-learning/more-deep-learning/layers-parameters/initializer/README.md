<h1>initializer</h1>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Enum.Png" src="assets/enum.png" width="42"/></td>
      <td valign="top"><strong>initializer :</strong> <em><strong>enum</strong></em>, defines how model weights are set before training, which can influence the speed and quality of convergence.</td>
    </tr>
  </tbody>
</table>

<h4>Constant</h4>

<p>Initializer that generates tensors with constant values.</p>

<h4>GlorotNormal</h4>

<p>The Glorot normal initializer, also called Xavier normal initializer. Draws samples from a truncated normal distribution centered on 0 with <strong><em>stddev = sqrt(2 / (fan_in + fan_out))</em></strong> where <em>fan_in</em> is the number of input units in the weight tensor and <em>fan_out</em> is the number of output units in the weight tensor.</p>

<h4>GlorotUniform</h4>

<p>The Glorot uniform initializer, also called Xavier uniform initializer. Draws samples from a uniform distribution within <em>[-limit, limit]</em>, where <em><strong>limit = sqrt(6 / (fan_in + fan_out))</strong></em> (<em>fan_in</em> is the number of input units in the weight tensor and <em>fan_out</em> is the number of output units).</p>

<h4>HeNormal</h4>

<p>It draws samples from a truncated normal distribution centered on 0 with <strong><em>stddev = sqrt(2 / fan_in)</em></strong> where <em>fan_in</em> is the number of input units in the weight tensor.</p>

<h4>HeUniform</h4>

<p>Draws samples from a uniform distribution within <em>[-limit, limit]</em>, within <em><strong>limit = sqrt(6 / fan_in) </strong></em>(<em>fan_in</em> is the number of input units in the weight tensor).</p>

<h4>Identity</h4>

<p>Only usable for generating 2D matrices.</p>

<h4>LecunNormal</h4>

<p>Initializers allow you to pre-specify an initialization strategy, encoded in the Initializer object, without knowing the shape and dtype of the variable being initialized.<br/>Draws samples from a truncated normal distribution centered on 0 with <strong><em>stddev = sqrt(1 / fan_in) </em></strong>where <em>fan_in </em>is the number of input units in the weight tensor.</p>

<h4>LecunUniform</h4>

<p>Draws samples from a uniform distribution within <em>[-limit, limit]</em>, where <strong><em>limit = sqrt(3 / fan_in) </em></strong>(<em>fan_in </em>is the number of input units in the weight tensor).</p>

<h4>Ones</h4>

<p>Initializer that generates tensors initialized to 1.​</p>

<h4>Orthogonal</h4>

<p>Initializer that generates an orthogonal matrix. If the shape of the tensor to initialize is two-dimensional, it is initialized with an orthogonal matrix obtained from the QR decomposition of a matrix of random numbers drawn from a normal distribution. If the matrix has fewer rows than columns then the output will have orthogonal rows. Otherwise, the output will have orthogonal columns.<br/>If the shape of the tensor to initialize is more than two-dimensional, a matrix of shape <em><strong>(shape[0] * … * shape[n – 2], shape[n – 1 ])</strong></em> is initialized, where <em>n</em> is the length of the shape vector. The matrix is subsequently reshaped to give a tensor of the desired shape.</p>

<h4>RandomNormal</h4>

<p>Draws samples from a uniform distribution for given parameters.</p>

<h4>RandomUniform</h4>

<p>Draws samples from a uniform distribution for given parameters.</p>

<h4>TruncatedNormal</h4>

<p>Initializer that generates a truncated normal distribution. The values generated are similar to values from a RandomNormal initializer except that values more than two standard deviations from the mean are discarded and re-drawn.</p>

<h4>VarianceScaling</h4>

<p>Initializer that adapts its scale to the shape of its input tensors. With distribution = <em>“truncated_normal”</em> or <em>“untruncated_normal”</em>, samples are drawn from a truncated/untruncated normal distribution with a mean of zero and a standard deviation (after truncation, if used) <em><strong>stddev = sqrt(scale / n)</strong></em>, where <em>n</em> is:</p>

<ul>
<li>number of input units in the weight tensor, <em>if mode = “fan_in”</em></li>
<li>number of output units, if <em>mode = “fan_out”</em></li>
<li>average of the numbers of input and output units, if <em>mode = “fan_avg”</em></li>
</ul>

<p>With distribution = <em>“uniform”</em>, samples are drawn from a uniform distribution within <em>[-limit, limit]</em><code></code>, where <em><strong>limit = sqrt(3 * scale / n)</strong></em>.</p>

<h4>Zeros</h4>

<p>Initializer that generates tensors initialized to 0.</p>
