<h1>VarianceScaling</h1>

<h2>Description</h2>

<p>Initializer that adapts its scale to the shape of its input tensors. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img src="../../../../../_resolved/and/assets/cluster.png" alt="Cluster.Png" width="231" /></p>

<p>With distribution = <em>“truncated_normal”</em> or <em>“untruncated_normal”</em>, samples are drawn from a truncated/untruncated normal distribution with a mean of zero and a standard deviation (after truncation, if used) <em><strong>stddev = sqrt(scale / n)</strong></em>, where <em>n</em> is:</p>

<ul>
<li>
<ul>
<li>number of input units in the weight tensor, <em>if mode = “fan_in”</em></li>
<li>number of output units, if <em>mode = “fan_out”</em></li>
<li>average of the numbers of input and output units, if <em>mode = “fan_avg”</em></li>
</ul>
</li>
</ul>

<p>With distribution = <em>“uniform”</em>, samples are drawn from a uniform distribution within <em>[-limit, limit]</em><code></code>, where <em><strong>limit = sqrt(3 * scale / n)</strong></em>.</p>

<table>
  <tbody>
    <tr>
      <td valign="top" width="70%"><h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Numeric Cluster.Png" src="assets/numeric-cluster.png" width="42"/></td>
      <td valign="top"><strong>Parameters : <i>cluster,</i></strong></td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Enum.Png" src="assets/enum.png" width="42"/></td>
      <td valign="top"><strong>mode : <em>enum,</em></strong> one of <code>"fan_in"</code>, <code>"fan_out"</code>, <code>"fan_avg"</code>.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Enum.Png" src="assets/enum.png" width="42"/></td>
      <td valign="top"><strong>distrib : <em>enum,</em></strong> random distribution to use. One of <code>"truncated_normal"</code>, <code>"untruncated_normal"</code>, or <code>"uniform"</code>.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Single.Png" src="assets/single.png" width="42"/></td>
      <td valign="top"><strong>scale : <em>float,</em></strong> scaling factor.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Integer 32.Png" src="assets/integer-32.png" width="42"/></td>
      <td valign="top"><strong>seed : <em>integer, </em></strong>used to make the behavior of the initializer deterministic. Note that an initializer seeded with an integer or -1 (unseeded) will produce the same random values across multiple calls.</td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img alt="variance_scaling_param" src="assets/variance_scaling_param.png" width="220"/></p></td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td valign="top" width="75%"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Cluster Out.Png" src="assets/cluster-out.png" width="42"/></td>
      <td valign="top"><strong>Initializer :</strong> <em><strong>cluster,</strong></em> this cluster defines the weight initialization strategy for a model.</td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="enum.png" src="assets/enum.png" width="42"/></td>
      <td valign="top"><strong><a href="../../../../more-deep-learning/layers-parameters/initializer/README.md">enum</a> :</strong> <em><strong>enum</strong></em>, an enumeration indicating the initialization type (e.g., Zeros, Glorot, HeNormal, etc.). If <code>enum</code> is set to <code>CustomInitializer</code>, the custom class on the right will be used. Otherwise, the selected initialization strategy will be applied with default parameters.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="output_object.png" src="assets/output_object.png" width="42"/></td>
      <td valign="top"><strong>Class :</strong> <em><strong>object</strong></em>, a custom initializer class instance.</td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="25%"><p align="center"><img alt="output_init" src="assets/output_init.png" width="220"/></p></td>
    </tr>
  </tbody>
</table>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>

<p align="center"><img alt="initializer_exemple" src="assets/initializer_exemple.png" width="220"/></p>
