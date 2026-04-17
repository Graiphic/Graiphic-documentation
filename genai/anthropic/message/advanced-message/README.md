<h1>Advanced Message</h1>

<h2>Description</h2>

<p>Send a structured list of input messages with text and/or image content, and the model will generate the next message in the conversation. The Messages API can be used for either single queries or stateless multi-turn conversations. Type : polymorphic.</p>

<p align="center"><img src="assets/advanced-message.png" alt="Advanced Message" width="270" /></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Anthropic in" src="assets/cAnthropiclvclass.png" width="42"/></td>
      <td valign="top"><strong>Anthropic in : <em>class</em></strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="json_request" src="assets/cstr.png" width="42"/></td>
      <td valign="top"><strong>json_request : <em>string</em></strong></td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Anthropic out" src="assets/iAnthropiclvclass.png" width="42"/></td>
      <td valign="top"><strong>Anthropic out : <em>class</em></strong></td>
    </tr>
  </tbody>
</table>

<table>
  <tbody>
    <tr>
      <td valign="top" width="100%"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="response" src="assets/icclst.png" width="42"/></td>
      <td valign="top"><strong>response : <em>cluster</em></strong>
<ul>
  <li><img alt="id" src="assets/istr.png" width="32"/> <strong>id : <em>string</em></strong></li>
  <li><img alt="type" src="assets/istr.png" width="32"/> <strong>type : <em>string</em></strong></li>
  <li><img alt="role" src="assets/istr.png" width="32"/> <strong>role : <em>string</em></strong></li>
  <li><img alt="model" src="assets/istr.png" width="32"/> <strong>model : <em>string</em></strong></li>
  <li><img alt="content" src="assets/i1dcclst.png" width="32"/> <strong>content : <em>array of cluster</em></strong>
<ul>
  <li><img alt="type" src="assets/istr.png" width="32"/> <strong>type : <em>string</em></strong></li>
  <li><img alt="text" src="assets/istr.png" width="32"/> <strong>text : <em>string</em></strong></li>
</ul></li>
  <li><img alt="stop_reason" src="assets/istr.png" width="32"/> <strong>stop_reason : <em>string</em></strong></li>
  <li><img alt="stop_sequence" src="assets/istr.png" width="32"/> <strong>stop_sequence : <em>string</em></strong></li>
  <li><img alt="usage" src="assets/inclst.png" width="32"/> <strong>usage : <em>cluster</em></strong>
<ul>
  <li><img alt="input_tokens" src="assets/iu32.png" width="32"/> <strong>input_tokens : <em>integer</em></strong></li>
  <li><img alt="cache_creation_input_tokens" src="assets/iu32.png" width="32"/> <strong>cache_creation_input_tokens : <em>integer</em></strong></li>
  <li><img alt="cache_read_input_tokens" src="assets/iu32.png" width="32"/> <strong>cache_read_input_tokens : <em>integer</em></strong></li>
  <li><img alt="output_tokens" src="assets/iu32.png" width="32"/> <strong>output_tokens : <em>integer</em></strong></li>
</ul></li>
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
      <td width="64" valign="top"><img alt="last_response" src="assets/istr.png" width="42"/></td>
      <td valign="top"><strong>last_response : <em>string</em></strong></td>
    </tr>
  </tbody>
</table>
