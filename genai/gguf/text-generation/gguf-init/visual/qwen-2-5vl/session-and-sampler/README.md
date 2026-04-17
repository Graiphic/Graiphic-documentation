<h1>Session And Sampler</h1>

<h2>Description</h2>

<p>Initialize a session and its sampler Type : polymorphic.</p>

<p align="center"><img alt="Session and Sampler" src="assets/Session and Sampler.png" width="270"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td valign="top" width="70%"><p><img alt="Session Parameters" src="assets/ccclst.png" width="32"/> <strong>Session Parameters : <em>cluster</em></strong></p>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Model File Path" src="assets/cpath.png" width="42"/></td>
      <td valign="top"><strong>Model File Path : <em>path</em></strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="MMProj File Path" src="assets/cpath.png" width="42"/></td>
      <td valign="top"><strong>MMProj File Path : <em>path</em></strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="n cpu threads" src="assets/ci32.png" width="42"/></td>
      <td valign="top"><strong>n cpu threads : <em>integer</em></strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="nb gpu layers" src="assets/ci32.png" width="42"/></td>
      <td valign="top"><strong>nb gpu layers : <em>integer</em></strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="n_ctx" src="assets/ci32.png" width="42"/></td>
      <td valign="top"><strong>n_ctx : <em>integer</em></strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="system prompt" src="assets/cstr.png" width="42"/></td>
      <td valign="top"><strong>system prompt : <em>string</em></strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="always keep system prompt" src="assets/cbool.png" width="42"/></td>
      <td valign="top"><strong>always keep system prompt : <em>boolean</em></strong></td>
    </tr>
  </tbody>
</table>
      </td>
      <td valign="top" width="30%"><p align="center"><img alt="Session Parameters" src="assets/Session Parameters.png" width="220"/></p></td>
    </tr>
  </tbody>
</table>

<table>
  <tbody>
    <tr>
      <td valign="top" width="70%"><p><img alt="Sampler Parameters" src="assets/cnclst.png" width="32"/> <strong>Sampler Parameters : <em>cluster</em></strong></p>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="temperature" src="assets/csgl.png" width="42"/></td>
      <td valign="top"><strong>temperature : <em>float</em></strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="top_p" src="assets/csgl.png" width="42"/></td>
      <td valign="top"><strong>top_p : <em>float</em></strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="min_p" src="assets/csgl.png" width="42"/></td>
      <td valign="top"><strong>min_p : <em>float</em></strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="top_k" src="assets/ci32.png" width="42"/></td>
      <td valign="top"><strong>top_k : <em>integer</em></strong></td>
    </tr>
  </tbody>
</table>
      </td>
      <td valign="top" width="30%"><p align="center"><img alt="Sampler Parameters" src="assets/Sampler Parameters.png" width="220"/></p></td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Qwen25VL out" src="assets/iQwen25VLlvclass.png" width="42"/></td>
      <td valign="top"><strong>Qwen25VL out : <em>class</em></strong></td>
    </tr>
  </tbody>
</table>
