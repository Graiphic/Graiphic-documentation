<h1>OneHotIoU</h1>

<h2>Description</h2>

<p>Computes the Intersection-Over-Union metric for one-hot encoded labels. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="one_hot_iou.png" src="assets/one_hot_iou.png" width="460"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Array Single.Png" src="assets/array-single.png" width="42"/></td>
      <td valign="top"><strong>y_pred : <em>array, </em></strong>predicted values.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Array Single.Png" src="assets/array-single.png" width="42"/></td>
      <td valign="top"><strong>y_true : <em>array, </em></strong>true values (one hot encoding for example, [0, 0, 1] for 3-class problem).</td>
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
      <td valign="top"><strong> parameters : <em>cluster,</em></strong></td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Array Integer 32.Png" src="assets/array-integer-32.png" width="42"/></td>
      <td valign="top"><strong>target_class_ids : <em>array,</em></strong> list of target class ids for which the metric is returned.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Booleen.Png" src="assets/booleen.png" width="42"/></td>
      <td valign="top"><strong>sparse_y_pred : <em>boolean,</em></strong> whether predictions are encoded using integers or one hot logits. If True predictions are integers and if False, predictions are one hot logits and the argmax function will be used to determine each sample’s most likely associated label according to “axis” parameters.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Integer 32.Png" src="assets/integer-32.png" width="42"/></td>
      <td valign="top"><strong>axis : <em>integer,</em></strong> the dimension containing the logits.</td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img alt="one_hot_iou_param" src="assets/one_hot_iou_param.png" width="220"/></p></td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Out Single.Png" src="assets/out-single.png" width="42"/></td>
      <td valign="top"><strong>one_hot_iou : <em>float, </em></strong>result.</td>
    </tr>
  </tbody>
</table>

<h2>Calculation</h2>

<p>This metric can be used to compute IoU for multi-class classification tasks where the labels are one-hot encoded (the last axis should have one dimension per class). If the boolean parameter sparse_y_pred is set to true, this means that the predictions are not encoded in one-hot, but are sparse integers. Consequently, it is not necessary to convert them to integer format using argmax on the class axis. Otherwise, if sparse_y_pred is false, then the labels and predictions are first converted to integer format using argmax on the class axis before the IoU is calculated.</p>

<p>So, depending on the value of sparse_y_pred, OneHotIoU can accommodate both one-hot encoded predictions and sparse integer predictions.</p>

<p>Note that if there is only one channel in the labels and predictions, this class is identical to the <a href="../iou/README.md">IoU</a> class. In this case, use IoU instead.</p>

<table>
  <tbody>
    <tr>
      <td valign="top" width="62%"><p align="center"><img alt="False &amp; True" src="assets/False &amp; True.png" width="220"/></p></td>
      <td valign="top" width="38%"><p align="center"><img alt="binary_iou_calcul" src="assets/binary_iou_calcul.png" width="220"/></p></td>
    </tr>
  </tbody>
</table>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>

<h3>Easy to use with one_hot</h3>

<p align="center"><img alt="OneHotIoU_one_hot_y_pred" src="assets/OneHotIoU_one_hot_y_pred.png" width="220"/></p>

<h3>Easy to use with sparse</h3>

<p align="center"><img alt="OneHotIoU_sparse_y_pred" src="assets/OneHotIoU_sparse_y_pred.png" width="220"/></p>
