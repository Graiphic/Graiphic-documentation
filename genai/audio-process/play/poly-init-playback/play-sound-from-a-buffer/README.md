<h1>Play Sound From A Buffer</h1>

<h2>Description</h2>

<p>Play a Sound Buffer. Typically used alongside a TTS (Text-to-Speech) buffer. Type : polymorphic.</p>

<p align="center"><img src="assets/play-sound-from-a-buffer.png" alt="Play Sound From A Buffer" width="270" /></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Sound Buffer" src="assets/cu64.png" width="42"/></td>
      <td valign="top"><strong>Sound Buffer : <em>integer</em></strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Output Device" src="assets/cu16.png" width="42"/></td>
      <td valign="top"><strong>Output Device : <em>integer</em></strong></td>
    </tr>
  </tbody>
</table>

<table>
  <tbody>
    <tr>
      <td valign="top" width="100%"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Parameters" src="assets/cnclst.png" width="42"/></td>
      <td valign="top"><strong>Parameters : <em>cluster</em></strong>
<ul>
  <li><img alt="volume" src="assets/csgl.png" width="32"/> <strong>volume : <em>float</em></strong></li>
  <li><img alt="sampleRate" src="assets/ci32.png" width="32"/> <strong>sampleRate : <em>integer</em></strong></li>
  <li><img alt="Channels" src="assets/ci32.png" width="32"/> <strong>Channels : <em>integer</em></strong></li>
</ul></td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="PlayBuffer out" src="assets/iPlayBufferlvclass.png" width="42"/></td>
      <td valign="top"><strong>PlayBuffer out : <em>class</em></strong></td>
    </tr>
  </tbody>
</table>
