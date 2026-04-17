<h1>Orthogonal</h1>

<h2>Description</h2>

<p>Initializer that generates an orthogonal matrix. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="Orthogonal" src="assets/Orthogonal.png" width="210"/></p>

<p>Initializer that generates an orthogonal matrix. If the shape of the tensor to initialize is two-dimensional, it is initialized with an orthogonal matrix obtained from the QR decomposition of a matrix of random numbers drawn from a normal distribution. If the matrix has fewer rows than columns then the output will have orthogonal rows. Otherwise, the output will have orthogonal columns.</p>

<p>If the shape of the tensor to initialize is more than two-dimensional, a matrix of shape <em><strong>(shape[0] * … * shape[n – 2], shape[n – 1 ])</strong></em> is initialized, where <em>n</em> is the length of the shape vector. The matrix is subsequently reshaped to give a tensor of the desired shape.</p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Integer 32.Png" src="assets/integer-32.png" width="42"/></td>
      <td valign="top"><strong>seed : <em>integer, </em></strong>used to make the behavior of the initializer deterministic. Note that an initializer seeded with an integer or -1 (unseeded) will produce the same random values across multiple calls.</td>
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
      <td width="64" valign="top"><img alt="init_with_seed.png" src="assets/init_with_seed.png" width="42"/></td>
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
