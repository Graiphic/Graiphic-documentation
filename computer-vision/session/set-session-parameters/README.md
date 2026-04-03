<h1>Set Session Parameters</h1>

<h2>Description</h2>

<p>Sets a property in the session. Type : <em><strong>polymorphic</strong><strong>.</strong></em></p>

<p align="center"><img src="assets/set_session_param.png" alt="Set_Session_Param.Png" width="271" /></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Session.Png" src="assets/input_session.png" width="42"/></td>
      <td valign="top"><strong>Session Src : <em>class</em></strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Enum.Png" src="assets/input_enum.png" width="42"/></td>
      <td valign="top">Parameters Type :<em> enum, </em>Session generic properties identifier.
<ul>
<li>
<ul>
<li>CAP_PROP_POS_MSEC : Current position of the video file in milliseconds</li>
<li>CAP_PROP_POS_FRAMES : 0-based index of the frame to be decoded/captured next</li>
<li>CAP_PROP_POS_AVI_RATIO : Relative position of the video file : 0=start of the film, 1=end of the film</li>
<li>CAP_PROP_FRAME_WIDTH : Width of the frames in the video stream</li>
<li>CAP_PROP_FRAME_HEIGHT : Height of the frames in the video stream</li>
<li>CAP_PROP_FPS : Frame rate</li>
<li>CAP_PROP_FOURCC : 4-character code of codec</li>
<li>CAP_PROP_FRAME_COUNT : Number of frames in the video file</li>
<li>CAP_PROP_FORMAT : Format of the Mat objects</li>
<li>CAP_PROP_MODE : Backend-specific value indicating the current capture mode</li>
<li>CAP_PROP_BRIGHTNESS : Brightness of the image (only for those cameras that support)</li>
<li>CAP_PROP_CONTRAST : Contrast of the image (only for cameras)</li>
<li>CAP_PROP_SATURATION : Saturation of the image (only for cameras)</li>
<li>CAP_PROP_HUE : Hue of the image (only for cameras)</li>
<li>CAP_PROP_GAIN : Gain of the image (only for those cameras that support)</li>
<li>CAP_PROP_EXPOSURE : Exposure (only for those cameras that support)</li>
<li>CAP_PROP_CONVERT_RGB : Boolean flags indicating whether images should be converted to RGB</li>
<li>CAP_PROP_WHITE_BALANCE_BLUE_U : Currently unsupported</li>
<li>CAP_PROP_WHITE_BALANCE_RED_V : Currently unsupported</li>
<li>CAP_PROP_RECTIFICATION : Rectification flag for stereo cameras</li>
<li>CAP_PROP_SAR_NUM : Sample aspect ratio : num/den (num)</li>
<li>CAP_PROP_SAR_DEN : Sample aspect ratio : num/den (den)</li>
<li>CAP_PROP_BACKEND : Current backend. Read-only property</li>
<li>CAP_PROP_CHANNEL : Video input or Channel Number</li>
<li>CAP_PROP_AUTO_WB : enable/ disable auto white-balance</li>
<li>CAP_PROP_WB_TEMPERATURE : white-balance color temperature</li>
<li>CAP_PROP_CODEC_PIXEL_FORMAT : (read-only) codec’s pixel format</li>
<li>CAP_PROP_BITRATE : (read-only) Video bitrate in kbits/s</li>
<li>CAP_PROP_ORIENTATION_META : (read-only) Frame rotation defined by stream meta</li>
<li>CAP_PROP_ORIENTATION_AUTO : rotates output frames of CvCapture considering video file’s metadata</li>
</ul>
</li>
</ul></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Double.Png" src="assets/input_double.png" width="42"/></td>
      <td valign="top"><strong>Value : <em>float,</em></strong> value for the specified property.</td>
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
      <td width="64" valign="top"><img alt="Output_Boolean.Png" src="assets/output_boolean.png" width="42"/></td>
      <td valign="top"><strong>Succeed? : <em>boolean, </em></strong>true if the property is supported by backend used by the <strong>Session</strong> instance.</td>
    </tr>
  </tbody>
</table>

<h2>Examples</h2>

<p>All these examples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Computer Vision ​library to run it).</p>
