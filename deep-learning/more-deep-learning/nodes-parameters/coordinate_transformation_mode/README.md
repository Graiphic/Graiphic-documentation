<h1>coordinate_transformation_mode</h1>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Enum.Png" src="assets/enum.png" width="42"/></td>
      <td valign="top"><strong>coordinate_transformation_mode : <em>enum,</em></strong> this attribute describes how to transform the coordinate in the resized tensor to the coordinate in the original tensor.</td>
    </tr>
  </tbody>
</table>

<p>The coordinate of each dimension is transformed individually. Using axis <code>x</code> as an example:</p>

<ul>
  <li><code>x_resized</code> is the coordinate of axis <code>x</code> in the resized tensor.</li>
  <li><code>x_original</code> is the coordinate of axis <code>x</code> in the original tensor.</li>
  <li><code>length_original</code> is the length of the original tensor on axis <code>x</code>.</li>
  <li><code>length_resized</code> is the length of the resized tensor on axis <code>x</code>.</li>
  <li><code>scale = length_resized / length_original</code>.</li>
  <li><code>output_width</code> is the target length on axis <code>x</code>, which can be fractional when derived from a scale factor.</li>
  <li><code>output_width_int</code> is the effective output width as an integer.</li>
</ul>

<p>If <code>coordinate_transformation_mode</code> is <code>"half_pixel"</code>:</p>

```text
x_original = (x_resized + 0.5) / scale - 0.5
```

<p>If <code>coordinate_transformation_mode</code> is <code>"half_pixel_symmetric"</code>:</p>

```text
adjustment = output_width_int / output_width
center = input_width / 2
offset = center * (1 - adjustment)
x_ori = offset + (x + 0.5) / scale - 0.5
```

<p>If <code>coordinate_transformation_mode</code> is <code>"pytorch_half_pixel"</code>:</p>

```text
x_original = length_resized > 1 ? (x_resized + 0.5) / scale - 0.5 : 0
```

<p>If <code>coordinate_transformation_mode</code> is <code>"align_corners"</code>:</p>

```text
x_original = x_resized * (length_original - 1) / (length_resized - 1)
```

<p>If <code>coordinate_transformation_mode</code> is <code>"asymmetric"</code>:</p>

```text
x_original = x_resized / scale
```

<p>If <code>coordinate_transformation_mode</code> is <code>"tf_crop_and_resize"</code>:</p>

```text
x_original = length_resized > 1
  ? start_x * (length_original - 1) + x_resized * (end_x - start_x) * (length_original - 1) / (length_resized - 1)
  : 0.5 * (start_x + end_x) * (length_original - 1)
```
