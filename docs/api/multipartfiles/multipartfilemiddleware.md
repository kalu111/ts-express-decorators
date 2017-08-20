<header class="symbol-info-header">    <h1 id="multipartfilemiddleware">MultipartFileMiddleware</h1>    <label class="symbol-info-type-label class">Class</label>    <label class="api-type-label private">private</label><label class="api-type-label middleware">middleware</label>  </header>
<section class="symbol-info">      <table class="is-full-width">        <tbody>        <tr>          <th>Module</th>          <td>            <div class="lang-typescript">                <span class="token keyword">import</span> { MultipartFileMiddleware }                 <span class="token keyword">from</span>                 <span class="token string">"ts-express-decorators/lib/multipartfiles/middlewares/MultipartFileMiddleware"</span>                            </div>          </td>        </tr>        <tr>          <th>Source</th>          <td>            <a href="https://romakita.github.io/ts-express-decorators/#//blob/v2.0.9/src/multipartfiles/middlewares/MultipartFileMiddleware.ts#L0-L0">                multipartfiles/middlewares/MultipartFileMiddleware.ts            </a>        </td>        </tr>                </tbody>      </table>    </section>

### Overview

<pre><code class="typescript-lang"><span class="token keyword">class</span> MultipartFileMiddleware <span class="token keyword">implements</span> <a href="#api/common/mvc/imiddleware"><span class="token">IMiddleware</span></a> <span class="token punctuation">{</span>
    <span class="token keyword">constructor</span><span class="token punctuation">(</span>serverSettingsService<span class="token punctuation">:</span> <a href="#api/common/server/serversettingsservice"><span class="token">ServerSettingsService</span></a><span class="token punctuation">)</span><span class="token punctuation">;</span>
    <span class="token function">use</span><span class="token punctuation">(</span>endpoint<span class="token punctuation">:</span> <a href="#api/common/mvc/endpointmetadata"><span class="token">EndpointMetadata</span></a><span class="token punctuation">,</span> request<span class="token punctuation">:</span> Express.<a href="#api/common/mvc/request"><span class="token">Request</span></a><span class="token punctuation">,</span> response<span class="token punctuation">:</span> Express.<a href="#api/common/mvc/response"><span class="token">Response</span></a><span class="token punctuation">,</span> next<span class="token punctuation">:</span> <span class="token keyword">any</span><span class="token punctuation">)</span><span class="token punctuation">:</span> <span class="token keyword">any</span><span class="token punctuation">;</span>
<span class="token punctuation">}</span></code></pre>

### Members

<div class="method-overview"><pre><code class="typescript-lang"><span class="token function">use</span><span class="token punctuation">(</span>endpoint<span class="token punctuation">:</span> <a href="#api/common/mvc/endpointmetadata"><span class="token">EndpointMetadata</span></a><span class="token punctuation">,</span> request<span class="token punctuation">:</span> Express.<a href="#api/common/mvc/request"><span class="token">Request</span></a><span class="token punctuation">,</span> response<span class="token punctuation">:</span> Express.<a href="#api/common/mvc/response"><span class="token">Response</span></a><span class="token punctuation">,</span> next<span class="token punctuation">:</span> <span class="token keyword">any</span><span class="token punctuation">)</span><span class="token punctuation">:</span> <span class="token keyword">any</span></code></pre></div>