<h1>IoU</h1>

<h2>Description</h2>

<p>Computes the Intersection-Over-Union metric for specific target classes. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img alt="iou.png" src="assets/iou.png" width="460"/></p>

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
      <td valign="top"><strong>target_class_ids : <em>array,</em></strong> list of target class ids for which the metric is returned.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Booleen.Png" src="assets/booleen.png" width="42"/></td>
      <td valign="top"><strong>sparse_y_true : <em>boolean,</em></strong> whether labels are encoded using integers or one hot logits. If True labels are integers and if False, labels are one hot logits and the argmax function will be used to determine each sample’s most likely associated label according to “axis” parameters.</td>
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
      <td valign="top" width="30%"><p align="center"><img alt="iou_param" src="assets/iou_param.png" width="220"/></p></td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Out Single.Png" src="assets/out-single.png" width="42"/></td>
      <td valign="top"><strong>iou : <em>float, </em></strong>result.</td>
    </tr>
  </tbody>
</table>

<h2>Use cases</h2>

<p>The IoU metric, which stands for Intersection over Union, is a widely used metric in computer vision, specifically for object detection and semantic segmentation tasks. It measures the correspondence between two sets, which are usually two areas in an image. In the context of object detection, these two sets are usually the ground truth (the actual location of the object in the image) and the model prediction (the location of the object as predicted by the model).<a href="https://www.deepl.com/translator?utm_source=windows&amp;utm_medium=app&amp;utm_campaign=windows-share"></a></p>

<h2>Calculation</h2>

<p>This metric first computes IoUs for all individual classes, then returns the mean of IoUs for the classes that are specified by <em><strong>“target_class_ids”</strong></em>.</p>

<p>She gives a value between 0 and 1. A value of 0 means that there is no overlap at all, while a value of 1 means that there is perfect overlap (the two bounding boxes are exactly the same).</p>

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

<p align="center"><img alt="IoU_one_hot_y_true_y_pred" src="assets/IoU_one_hot_y_true_y_pred.png" width="220"/></p>

<h3>Easy to use with sparse</h3>

<p align="center"><img alt="IoU_sparse_y_true_y_pred" src="assets/IoU_sparse_y_true_y_pred.png" width="220"/></p>
