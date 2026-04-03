<h1>Create Llama Generator</h1>

<h2>Description</h2>

<p>Create Streaming Llama Generator Session.</p>

<p align="center"><img alt="output_object.png" src="assets/output_object.png" width="300"/></p>

<h3>Input parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Input_Object.Png" src="assets/input_object.png" width="42"/></td>
      <td valign="top"><strong>ONNX in : <em>object, </em></strong>llama generator session.</td>
    </tr>
  </tbody>
</table>

<table>
  <tbody>
    <tr>
      <td valign="top" width="70%"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Cluster.Png" src="assets/cluster.png" width="42"/></td>
      <td valign="top"><strong>Parameters : <em>cluster,</em></strong></td>
    </tr>
    <tr>
      <td></td>
      <td valign="top"><table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="Booleen.Png" src="assets/booleen.png" width="42"/></td>
      <td valign="top"><strong>use_position_ids :</strong> <em><strong>boolean</strong></em>, enables the use of explicit position IDs for the input tokens.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Single.Png" src="assets/single.png" width="42"/></td>
      <td valign="top"><strong>temperature :</strong> <em><strong>float</strong></em>, controls randomness in the generation process.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Single.Png" src="assets/single.png" width="42"/></td>
      <td valign="top"><strong>repetition_penalty :</strong> <em><strong>float</strong></em>, penalizes repeated tokens to reduce looping or redundant text.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Integer 32.Png" src="assets/integer-32.png" width="42"/></td>
      <td valign="top"><strong>max_length :</strong> <em><strong>integer</strong></em>, maximum number of tokens in the generated output sequence.</td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Integer 32.Png" src="assets/integer-32.png" width="42"/></td>
      <td valign="top"><strong>ngram_size :</strong> <em><strong>integer</strong></em>, size of n-grams tracked to prevent repetition.</td>
    </tr>
  </tbody>
</table></td>
    </tr>
    <tr>
      <td width="64" valign="top"><img alt="Input_Unsigned_64.Png" src="assets/input_unsigned_64.png" width="42"/></td>
      <td valign="top"><strong>llama_decoder_session : <em>integer, </em></strong>reference to an active ONNX inference session of the LLaMA decoder model.</td>
    </tr>
  </tbody>
</table></td>
      <td valign="top" width="30%"><p align="center"><img alt="param_llama_create" src="assets/param_llama_create.png" width="220"/></p></td>
    </tr>
  </tbody>
</table>

<h3>Output parameters</h3>

<table>
  <tbody>
    <tr>
      <td width="64" valign="top"><img alt="llama_create.png" src="assets/llama_create.png" width="42"/></td>
      <td valign="top"><strong>ONNX out : <em>object, </em></strong>llama generator session.</td>
    </tr>
  </tbody>
</table>

<h2>Example</h2>

<p>All these exemples are snippets PNG, you can drop these Snippet onto the block diagram and get the depicted code added to your VI (Do not forget to install Deep Learning library to run it).</p>
