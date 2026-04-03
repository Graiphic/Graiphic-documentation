<h1>Set Camera Mode</h1>

<h2>Description</h2>

<p>Modify the camera mode (Resolution and FPS). Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img src="assets/set_camera_modes.png" alt="Set_Camera_Modes.Png" width="327" /></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Session.Png" src="assets/input_session.png" width="42"/></td>
      <td valign="top"><strong>Session Src : <em>class</em></strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Interger_32.Png" src="assets/input_interger_32.png" width="42"/></td>
      <td valign="top">Camera Mode :<em> integer,</em> index for this video mode.</td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Output_Session.Png" src="assets/output_session.png" width="42"/></td>
      <td valign="top"><strong>Session Dst : <em>class</em></strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output_String.Png" src="assets/output_string.png" width="42"/></td>
      <td valign="top">Camera Mode Name :<em> string,</em> name of the video mode, such as <strong>160×90 MJPG 30,00 fps.</strong></td>
    </tr>
  </tbody>
</table>

<h2>Examples</h2>

<p>All these examples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Computer Vision ​library to run it).</p>

<h3>Opens and reads the camera in a defined mode</h3>

<p align="center"><img src="assets/get_set_camera_modes.png" alt="get_set_camera_modes" width="260" /></p>
