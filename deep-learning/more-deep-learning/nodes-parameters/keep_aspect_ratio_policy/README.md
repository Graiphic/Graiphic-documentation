<h1>keep_aspect_ratio_policy</h1>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Enum.Png" src="assets/enum.png" width="42"/></td>
      <td valign="top"><strong>keep_aspect_ratio_policy : <em>enum,</em></strong> this attribute describes how to interpret the <code>sizes</code> input with regard to keeping the original aspect ratio of the input, and it is not applicable when the <code>scales</code> input is used.</td>
    </tr>
  </tbody>
</table>

<p>Given a set of <code>sizes</code>, associated with a subset of <code>axes</code> (explicitly provided or default), assume <code>d = axes[i]</code>, where <code>i</code> is the index of the provided <code>sizes</code>.</p>

<p>If <code>keep_aspect_ratio_policy</code> is <code>"stretch"</code>, the original aspect ratio is disregarded, and the input is resized to the specified size:</p>

```text
out_size[d] = sizes[i]
```

<p>If <code>keep_aspect_ratio_policy</code> is <code>"not_larger"</code>, the sizes are adjusted so that no extent of the output is larger than the specified size, while keeping the original aspect ratio:</p>

```text
scale = Min(sizes[i] / in_size[d])
out_size[d] = round_int(scale * in_size[d])
```

<p>If <code>keep_aspect_ratio_policy</code> is <code>"not_smaller"</code>, the sizes are adjusted so that no extent of the output is smaller than the specified size, while keeping the original aspect ratio:</p>

```text
scale = Max(sizes[i] / in_size[d])
out_size[d] = round_int(scale * in_size[d])
```

<p>For non-resizable axes (those not specified in <code>axes</code>), the output size will be equal to the input size.</p>

<p>Note: <code>round_int</code> stands for computing the nearest integer value, rounding halfway cases up.</p>
