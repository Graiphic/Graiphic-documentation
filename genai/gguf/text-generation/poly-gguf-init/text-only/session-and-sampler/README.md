<h1>Session And Sampler</h1>

<h2>Description</h2>

<p>Initialize a session and its sampler Type : polymorphic.</p>

<p align="center"><img src="assets/session-and-sampler.png" alt="Session And Sampler" width="270" /></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td valign="top" width="100%"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Session Parameters" src="assets/ccclst.png" width="42"/></td>
      <td valign="top"><strong>Session Parameters : <em>cluster</em></strong>
<ul>
  <li><img alt="Model File Path" src="assets/cpath.png" width="32"/> <strong>Model File Path : <em>path</em></strong></li>
  <li><img alt="n cpu threads" src="assets/ci32.png" width="32"/> <strong>n cpu threads : <em>integer</em></strong></li>
  <li><img alt="nb gpu layers" src="assets/ci32.png" width="32"/> <strong>nb gpu layers : <em>integer</em></strong></li>
  <li><img alt="n_ctx" src="assets/ci32.png" width="32"/> <strong>n_ctx : <em>integer</em></strong></li>
  <li><img alt="system prompt" src="assets/cstr.png" width="32"/> <strong>system prompt : <em>string</em></strong></li>
  <li><img alt="always keep system prompt" src="assets/cbool.png" width="32"/> <strong>always keep system prompt : <em>boolean</em></strong></li>
</ul></td>
    </tr>
  </tbody>
</table></td>
    </tr>
  </tbody>
</table>

<table>
  <tbody>
    <tr>
      <td valign="top" width="100%"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Sampler Parameters" src="assets/cnclst.png" width="42"/></td>
      <td valign="top"><strong>Sampler Parameters : <em>cluster</em></strong>
<ul>
  <li><img alt="temperature" src="assets/csgl.png" width="32"/> <strong>temperature : <em>float</em></strong></li>
  <li><img alt="top_p" src="assets/csgl.png" width="32"/> <strong>top_p : <em>float</em></strong></li>
  <li><img alt="min_p" src="assets/csgl.png" width="32"/> <strong>min_p : <em>float</em></strong></li>
  <li><img alt="top_k" src="assets/ci32.png" width="32"/> <strong>top_k : <em>integer</em></strong></li>
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
      <td width="64" valign="top"><img alt="TextOnly out" src="assets/iTextOnlylvclass.png" width="42"/></td>
      <td valign="top"><strong>TextOnly out : <em>class</em></strong></td>
    </tr>
  </tbody>
</table>
