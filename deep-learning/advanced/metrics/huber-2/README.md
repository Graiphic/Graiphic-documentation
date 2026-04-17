<h1>Huber</h1>

<h2>Description</h2>

<p>Computes the huber metrics between y_true and y_pred. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="Huber" src="assets/huber.png" width="460"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Array Single.Png" src="assets/array-single.png" width="42"/></td>
      <td valign="top"><strong>y_pred : <em>array, </em></strong>predicted values.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Array Single.Png" src="assets/array-single.png" width="42"/></td>
      <td valign="top"><strong>y_true : <em>array, </em></strong>true values.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Single.Png" src="assets/single.png" width="42"/></td>
      <td valign="top"><strong>delta : <em>float,</em></strong> the point at which the loss changes from quadratic to linear.</td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Out Single.Png" src="assets/out-single.png" width="42"/></td>
      <td valign="top"><strong>huber : <em>float, </em></strong>result.</td>
    </tr>
  </tbody>
</table>

<h2>Use cases</h2>

<p>Huber’s loss function, also known as Huber’s robust loss, is a metric used in machine learning, particularly for regression problems. It is less sensitive to outliers than the root-mean-square loss, making it useful when there are large prediction errors. It is a function that is quadratic for small values, but linear for large values. This means that it tries to strike a balance between mean square loss (which strongly punishes large errors) and mean absolute loss (which is more robust to outliers).</p>

<p>This loss function is often used in the following areas :</p>

<ul>
<li>
<ul>
<li>Signal processing : for example, when there is noise in the data.</li>
<li>Computer vision : for example, when predicting the positions of objects in an image.</li>
<li>Financial analysis : for example, when predicting the price of shares or other financial securities, where there may be sudden, large price movements.</li>
<li>Robotics : for example, in control problems where models are used to predict forces or positions.</li>
</ul>
</li>
</ul>

<p>Note that the Huber loss function has a parameter called delta, which determines the point at which the loss changes from quadratic to linear. This parameter can be adjusted to control sensitivity to outliers.</p>

<h2>Calculation</h2>

<p>Essentially, the Huber loss is quadratic for small errors and linear for large errors. The threshold between small and large errors is a ‘delta’ hyperparameter that you can adjust.</p>

<p>The advantage of the Huber loss is that it does not penalise large errors as much as the quadratic loss, which makes it more robust to outliers. At the same time, it retains an important property of quadratic loss functions : it is differentiable, which makes it useful for optimisation.</p>

<p align="center"><img alt="huber_calcul" src="assets/huber_calcul.png" width="220"/></p>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>

<h3>Easy to use</h3>

<p align="center"><img alt="Huber" src="assets/huber.png" width="220"/></p>
