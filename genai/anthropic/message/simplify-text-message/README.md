<h1>Simplify Text Message</h1>

<h2>Description</h2>

<p>Send a structured list of input messages with text and/or image content, and the model will generate the next message in the conversation. The Messages API can be used for either single queries or stateless multi-turn conversations. Type : polymorphic.</p>

<p align="center"><img alt="Simplify Text Message" src="assets/Simplify Text Message.png" width="270"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Anthropic in" src="assets/cAnthropiclvclass.png" width="42"/></td>
      <td valign="top"><strong>Anthropic in : <em>class</em></strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="message" src="assets/cstr.png" width="42"/></td>
      <td valign="top"><strong>message : <em>string</em></strong></td>
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
      <td valign="top" width="70%"><p><img alt="response" src="assets/icclst.png" width="32"/> <strong>response : <em>cluster</em></strong></p>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="id" src="assets/istr.png" width="42"/></td>
      <td valign="top"><strong>id : <em>string</em></strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="type" src="assets/istr.png" width="42"/></td>
      <td valign="top"><strong>type : <em>string</em></strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="role" src="assets/istr.png" width="42"/></td>
      <td valign="top"><strong>role : <em>string</em></strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="model" src="assets/istr.png" width="42"/></td>
      <td valign="top"><strong>model : <em>string</em></strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="content" src="assets/i1dcclst.png" width="42"/></td>
      <td valign="top"><strong>content : <em>array of cluster</em></strong>
<ul>
  <li><img alt="type" src="assets/istr.png" width="32"/> <strong>type : <em>string</em></strong></li>
  <li><img alt="text" src="assets/istr.png" width="32"/> <strong>text : <em>string</em></strong></li>
</ul></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="stop_reason" src="assets/istr.png" width="42"/></td>
      <td valign="top"><strong>stop_reason : <em>string</em></strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="stop_sequence" src="assets/istr.png" width="42"/></td>
      <td valign="top"><strong>stop_sequence : <em>string</em></strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="usage" src="assets/inclst.png" width="42"/></td>
      <td valign="top"><strong>usage : <em>cluster</em></strong>
<ul>
  <li><img alt="input_tokens" src="assets/iu32.png" width="32"/> <strong>input_tokens : <em>integer</em></strong></li>
  <li><img alt="cache_creation_input_tokens" src="assets/iu32.png" width="32"/> <strong>cache_creation_input_tokens : <em>integer</em></strong></li>
  <li><img alt="cache_read_input_tokens" src="assets/iu32.png" width="32"/> <strong>cache_read_input_tokens : <em>integer</em></strong></li>
  <li><img alt="output_tokens" src="assets/iu32.png" width="32"/> <strong>output_tokens : <em>integer</em></strong></li>
</ul></td>
    </tr>
  </tbody>
</table>
      </td>
      <td valign="top" width="30%"><p align="center"><img alt="response" src="assets/response.png" width="220"/></p></td>
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
