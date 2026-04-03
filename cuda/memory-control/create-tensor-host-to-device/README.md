<h1>Create Tensor & Host To Device</h1>

<h2>Description</h2>

<p>Allocates size bytes of linear memory on the device and copies data between host and device. Returns a tensor to the allocated memory. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img src="assets/create_tensor_and_host_to_device.png" alt="Create_Tensor_And_Host_To_Device.Png" width="219" /></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Array_Single.Png" src="assets/input_array_single.png" width="42"/></td>
      <td valign="top"><strong>data : <em>array, </em></strong>data copied on the device (can be a scalar, 1D, 2D, 3D, 4D, 5D, 6D array).</td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Tensor.Png" src="assets/output_tensor.png" width="42"/></td>
      <td valign="top"><strong>Tensor out : <i>class</i></strong></td>
    </tr>
  </tbody>
</table>

<h2>Examples</h2>

<p>All these examples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Accelerator library to run it).</p>

<p align="center"><img src="assets/ex_mem_control_1.png" alt="ex_mem_control_1" width="260" /></p>
