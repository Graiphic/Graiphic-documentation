<h1>Accuracy</h1>

<h2>Description</h2>

<p>Calculates how often predictions equal labels. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="accuracy.PNG" src="assets/accuracy.PNG" width="460"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Array Integer 32.Png" src="assets/array-integer-32.png" width="42"/></td>
      <td valign="top"><strong>  y_pred : <em>array, </em></strong>predicted values (numerical label for example, [ 0 ], [ 1 ] and [ 2 ] for 3-class problem).</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Array Integer 32.Png" src="assets/array-integer-32.png" width="42"/></td>
      <td valign="top"><strong>y_true : <em>array, </em></strong>true values (numerical label for example, [ 0 ], [ 1 ] and [ 2 ] for 3-class problem).</td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Out Single.Png" src="assets/out-single.png" width="42"/></td>
      <td valign="top"><strong>accuracy : <em>float, </em></strong>result.</td>
    </tr>
  </tbody>
</table>

<h2>Use cases</h2>

<p>Accuracy is a performance measure commonly used in machine learning, natural language processing (NLP) and computer vision. It is generally used when the output classes of a classification model are equally balanced.</p>

<p>It can be used to evaluate a model in various scenarios, for example :</p>

<ul>
<li>
<ul>
<li>Binary classification : where an output variable can be either 0 or 1. For example, to determine whether an email is spam or not.</li>
<li>Multiclass classification : where an output variable can have more than two possible states. For example, to predict the breed of a dog from an image.</li>
</ul>
</li>
</ul>

<h2>Calculation</h2>

<p>Computes the frequency with which y_pred matches y_true. This frequency is ultimately returned as binary accuracy : an idempotent operation that simply divides total by count.</p>

<p align="center"><img alt="accuracy_calcul" src="assets/accuracy_calcul.PNG" width="220"/></p>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>

<h3>Easy to use</h3>

<p align="center"><img alt="Accuracy" src="assets/accuracy.PNG" width="220"/></p>
