<h1>Simplify Text Message</h1>

<!-- GENAI_EXPERIMENTAL_NOTICE_START -->
<blockquote>
<p><strong>Experimental documentation.</strong> This GenAI Toolkit page is experimental and may change significantly while the toolkit is being validated.</p>
</blockquote>
<!-- GENAI_EXPERIMENTAL_NOTICE_END -->

<h2>Description</h2>

<p>Send a structured list of input messages with text and/or image content, and the model will generate the next message in the conversation. The Messages API can be used for either single queries or stateless multi-turn conversations. Type : polymorphic.</p>

<p align="center"><img src="assets/simplify-text-message.png" alt="Simplify Text Message" width="270" /></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Anthropic in" src="assets/cAnthropiclvclass.png" width="42"/></td>
      <td valign="top"><strong>Anthropic in</strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="message" src="assets/cstr.png" width="42"/></td>
      <td valign="top"><strong>message</strong></td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Anthropic out" src="assets/iAnthropiclvclass.png" width="42"/></td>
      <td valign="top"><strong>Anthropic out</strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="response" src="assets/icclst.png" width="42"/></td>
      <td valign="top"><strong>response</strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="response.id" src="assets/istr.png" width="42"/></td>
      <td valign="top"><strong>response.id</strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="response.type" src="assets/istr.png" width="42"/></td>
      <td valign="top"><strong>response.type</strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="response.role" src="assets/istr.png" width="42"/></td>
      <td valign="top"><strong>response.role</strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="response.model" src="assets/istr.png" width="42"/></td>
      <td valign="top"><strong>response.model</strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="response.content" src="assets/i1dcclst.png" width="42"/></td>
      <td valign="top"><strong>response.content</strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="response.content[].type" src="assets/istr.png" width="42"/></td>
      <td valign="top"><strong>response.content[].type</strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="response.content[].text" src="assets/istr.png" width="42"/></td>
      <td valign="top"><strong>response.content[].text</strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="response.stop_reason" src="assets/istr.png" width="42"/></td>
      <td valign="top"><strong>response.stop_reason</strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="response.stop_sequence" src="assets/istr.png" width="42"/></td>
      <td valign="top"><strong>response.stop_sequence</strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="response.usage" src="assets/inclst.png" width="42"/></td>
      <td valign="top"><strong>response.usage</strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="response.usage.input_tokens" src="assets/iu32.png" width="42"/></td>
      <td valign="top"><strong>response.usage.input_tokens</strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="response.usage.cache_creation_input_tokens" src="assets/iu32.png" width="42"/></td>
      <td valign="top"><strong>response.usage.cache_creation_input_tokens</strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="response.usage.cache_read_input_tokens" src="assets/iu32.png" width="42"/></td>
      <td valign="top"><strong>response.usage.cache_read_input_tokens</strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="response.usage.output_tokens" src="assets/iu32.png" width="42"/></td>
      <td valign="top"><strong>response.usage.output_tokens</strong></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="last_response" src="assets/istr.png" width="42"/></td>
      <td valign="top"><strong>last_response</strong></td>
    </tr>
  </tbody>
</table>
