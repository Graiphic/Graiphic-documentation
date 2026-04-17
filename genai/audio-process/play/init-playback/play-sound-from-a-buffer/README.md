<h1>Play Sound From A Buffer</h1>

<h2>Description</h2>

<p>Play a Sound Buffer. Typically used alongside a TTS (Text-to-Speech) buffer. Type : polymorphic.</p>

<p align="center"><img alt="Play Sound From a Buffer" src="assets/Play Sound From a Buffer.png" width="270"/></p>

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
      <td valign="top" width="70%"><p><img alt="Parameters" src="assets/cnclst.png" width="32"/> <strong>Parameters : <em>cluster</em></strong></p>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="volume" src="assets/csgl.png" width="42"/></td>
      <td valign="top"><strong>volume : <em>float</em></strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="sampleRate" src="assets/ci32.png" width="42"/></td>
      <td valign="top"><strong>sampleRate : <em>integer</em></strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Channels" src="assets/ci32.png" width="42"/></td>
      <td valign="top"><strong>Channels : <em>integer</em></strong></td>
    </tr>
  </tbody>
</table>
      </td>
      <td valign="top" width="30%"><p align="center"><img alt="Parameters" src="assets/Parameters.png" width="220"/></p></td>
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
