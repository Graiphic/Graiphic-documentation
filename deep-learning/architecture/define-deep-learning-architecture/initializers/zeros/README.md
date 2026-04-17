<h1>Zeros</h1>

<h2>Description</h2>

<p>Initializer that generates tensors initialized to 0. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="Zeros" src="assets/Zeros.png" width="210"/></p>

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
      <td width="64" valign="top"><img alt="init.png" src="assets/init.png" width="42"/></td>
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
