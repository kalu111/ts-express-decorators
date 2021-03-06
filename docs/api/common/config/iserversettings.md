
<header class="symbol-info-header"><h1 id="iserversettings">IServerSettings</h1><label class="symbol-info-type-label interface">Interface</label></header>
<!-- summary -->
<section class="symbol-info"><table class="is-full-width"><tbody><tr><th>Module</th><td><div class="lang-typescript"><span class="token keyword">import</span> { IServerSettings }&nbsp;<span class="token keyword">from</span>&nbsp;<span class="token string">"@tsed/common"</span></div></td></tr><tr><th>Source</th><td><a href="https://github.com/Romakita/ts-express-decorators/blob/v4.23.1/src//common/config/interfaces/IServerSettings.ts#L0-L0">/common/config/interfaces/IServerSettings.ts</a></td></tr></tbody></table></section>
<!-- overview -->


### Overview


<pre><code class="typescript-lang "><span class="token keyword">interface</span> IServerSettings <span class="token punctuation">{</span>
    rootDir?<span class="token punctuation">:</span> <span class="token keyword">string</span><span class="token punctuation">;</span>
    env?<span class="token punctuation">:</span> <a href="#api/core/env"><span class="token">Env</span></a><span class="token punctuation">;</span>
    port?<span class="token punctuation">:</span> <span class="token keyword">string</span> | <span class="token keyword">number</span><span class="token punctuation">;</span>
    httpPort?<span class="token punctuation">:</span> <span class="token keyword">string</span> | <span class="token keyword">number</span> | false<span class="token punctuation">;</span>
    httpsPort?<span class="token punctuation">:</span> <span class="token keyword">string</span> | <span class="token keyword">number</span> | false<span class="token punctuation">;</span>
    httpsOptions?<span class="token punctuation">:</span> Https.ServerOptions<span class="token punctuation">;</span>
    uploadDir?<span class="token punctuation">:</span> <span class="token keyword">string</span><span class="token punctuation">;</span>
    mount?<span class="token punctuation">:</span> <a href="#api/common/config/iservermountdirectories"><span class="token">IServerMountDirectories</span></a><span class="token punctuation">;</span>
    componentsScan?<span class="token punctuation">:</span> <span class="token keyword">string</span><span class="token punctuation">[</span><span class="token punctuation">]</span><span class="token punctuation">;</span>
    exclude?<span class="token punctuation">:</span> <span class="token keyword">string</span><span class="token punctuation">[</span><span class="token punctuation">]</span><span class="token punctuation">;</span>
    serveStatic?<span class="token punctuation">:</span> <a href="#api/common/config/iservermountdirectories"><span class="token">IServerMountDirectories</span></a><span class="token punctuation">;</span>
    acceptMimes?<span class="token punctuation">:</span> <span class="token keyword">string</span><span class="token punctuation">[</span><span class="token punctuation">]</span><span class="token punctuation">;</span>
    debug?<span class="token punctuation">:</span> <span class="token keyword">boolean</span><span class="token punctuation">;</span>
    logRequestFields?<span class="token punctuation">:</span> <span class="token punctuation">(</span>"reqId" | "method" | "url" | "headers" | "body" | "query" | "params" | "duration"<span class="token punctuation">)</span><span class="token punctuation">[</span><span class="token punctuation">]</span><span class="token punctuation">;</span>
    validationModelStrict?<span class="token punctuation">:</span> <span class="token keyword">boolean</span><span class="token punctuation">;</span>
    logger?<span class="token punctuation">:</span> Partial<<a href="#api/common/config/iloggersettings"><span class="token">ILoggerSettings</span></a>><span class="token punctuation">;</span>
    errors?<span class="token punctuation">:</span> Partial<<a href="#api/common/config/ierrorssettings"><span class="token">IErrorsSettings</span></a>><span class="token punctuation">;</span>
    controllerScope?<span class="token punctuation">:</span> <a href="#api/common/di/providerscope"><span class="token">ProviderScope</span></a><span class="token punctuation">;</span>
    routers?<span class="token punctuation">:</span> <a href="#api/common/config/iroutersettings"><span class="token">IRouterSettings</span></a><span class="token punctuation">;</span>
    <span class="token punctuation">[</span>key<span class="token punctuation">:</span> <span class="token keyword">string</span><span class="token punctuation">]</span><span class="token punctuation">:</span> <span class="token keyword">any</span><span class="token punctuation">;</span>
<span class="token punctuation">}</span></code></pre>


<!-- Parameters -->

<!-- Description -->

<!-- Members -->







### Members



<div class="method-overview">
<pre><code class="typescript-lang ">rootDir?<span class="token punctuation">:</span> <span class="token keyword">string</span></code></pre>
</div>


The root directory where you build run project. By default, it's equal to `process.cwd().



<hr/>



<div class="method-overview">
<pre><code class="typescript-lang ">env?<span class="token punctuation">:</span> <a href="#api/core/env"><span class="token">Env</span></a></code></pre>
</div>


The environment profile. By default the environment profile is equals to `NODE_ENV`.



<hr/>



<div class="method-overview">
<pre><code class="typescript-lang ">port?<span class="token punctuation">:</span> <span class="token keyword">string</span> | <span class="token keyword">number</span></code></pre>
</div>


Port number for the [HTTP.Server](https://nodejs.org/api/http.html#http_class_http_server).



<hr/>



<div class="method-overview">
<pre><code class="typescript-lang ">httpPort?<span class="token punctuation">:</span> <span class="token keyword">string</span> | <span class="token keyword">number</span> | false</code></pre>
</div>


Port number for the [HTTP.Server](https://nodejs.org/api/http.html#http_class_http_server).



<hr/>



<div class="method-overview">
<pre><code class="typescript-lang ">httpsPort?<span class="token punctuation">:</span> <span class="token keyword">string</span> | <span class="token keyword">number</span> | false</code></pre>
</div>


Port number for the [HTTPs.Server](https://nodejs.org/api/https.html#https_class_https_server).



<hr/>



<div class="method-overview">
<pre><code class="typescript-lang ">httpsOptions?<span class="token punctuation">:</span> Https.ServerOptions</code></pre>
</div>


[Https.ServerOptions](https://nodejs.org/api/tls.html#tls_tls_createserver_options_secureconnectionlistener)):
- `key` &lt;string&gt; | &lt;string[]&gt; | [&lt;Buffer&gt;](https://nodejs.org/api/buffer.html#buffer_class_buffer) | &lt;Object[]&gt;: The private key of the server in PEM format. To support multiple keys using different algorithms an array can be provided either as a plain array of key strings or an array of objects in the format `{pem: key, passphrase: passphrase}`. This option is required for ciphers that make use of private keys.
- `passphrase` &lt;string&gt; A string containing the passphrase for the private key or pfx.
- `cert` &lt;string&gt; | &lt;string[]&gt; | [&lt;Buffer&gt;](https://nodejs.org/api/buffer.html#buffer_class_buffer) | [&lt;Buffer[]&gt;](https://nodejs.org/api/buffer.html#buffer_class_buffer): A string, Buffer, array of strings, or array of Buffers containing the certificate key of the server in PEM format. (Required)
- `ca` &lt;string&gt; | &lt;string[]&gt; | [&lt;Buffer&gt;](https://nodejs.org/api/buffer.html#buffer_class_buffer) | [&lt;Buffer[]&gt;](https://nodejs.org/api/buffer.html#buffer_class_buffer): A string, Buffer, array of strings, or array of Buffers of trusted certificates in PEM format. If this is omitted several well known "root" CAs (like VeriSign) will be used. These are used to authorize connections.



<hr/>



<div class="method-overview">
<pre><code class="typescript-lang ">uploadDir?<span class="token punctuation">:</span> <span class="token keyword">string</span></code></pre>
</div>


The temporary directory to upload the documents. See more on [Upload file with Multer](tutorials/upload-files-with-multer.md)



<hr/>



<div class="method-overview">
<pre><code class="typescript-lang ">mount?<span class="token punctuation">:</span> <a href="#api/common/config/iservermountdirectories"><span class="token">IServerMountDirectories</span></a></code></pre>
</div>


Mount all controllers under a directories to an endpoint.



<hr/>



<div class="method-overview">
<pre><code class="typescript-lang ">componentsScan?<span class="token punctuation">:</span> <span class="token keyword">string</span><span class="token punctuation">[</span><span class="token punctuation">]</span></code></pre>
</div>


List of directories to scan [Services](docs/services/overview.md), [Middlewares](docs/middlewares/overview.md) or [Converters](docs/converters.md).



<hr/>



<div class="method-overview">
<pre><code class="typescript-lang ">exclude?<span class="token punctuation">:</span> <span class="token keyword">string</span><span class="token punctuation">[</span><span class="token punctuation">]</span></code></pre>
</div>


List of glob patterns. Exclude all files which matching with this list when ServerLoader scan all components with the `mount` or `scanComponents` options.



<hr/>



<div class="method-overview">
<pre><code class="typescript-lang ">serveStatic?<span class="token punctuation">:</span> <a href="#api/common/config/iservermountdirectories"><span class="token">IServerMountDirectories</span></a></code></pre>
</div>


Object to mount all directories under to his endpoints. See more on [Serve Static](tutorials/serve-static-files.md).



<hr/>



<div class="method-overview">
<pre><code class="typescript-lang ">acceptMimes?<span class="token punctuation">:</span> <span class="token keyword">string</span><span class="token punctuation">[</span><span class="token punctuation">]</span></code></pre>
</div>


Configure the mimes accepted by default by the server.



<hr/>



<div class="method-overview">
<pre><code class="typescript-lang ">debug?<span class="token punctuation">:</span> <span class="token keyword">boolean</span></code></pre>
</div>


Enable debug mode. By default debug is false.



<hr/>



<div class="method-overview">
<pre><code class="typescript-lang deprecated ">logRequestFields?<span class="token punctuation">:</span> <span class="token punctuation">(</span>"reqId" | "method" | "url" | "headers" | "body" | "query" | "params" | "duration"<span class="token punctuation">)</span><span class="token punctuation">[</span><span class="token punctuation">]</span></code></pre>
</div>




<hr/>



<div class="method-overview">
<pre><code class="typescript-lang ">validationModelStrict?<span class="token punctuation">:</span> <span class="token keyword">boolean</span></code></pre>
</div>


Use a strict validation when a model is used by the converter.
When a property is unknown, it throw a `BadRequest` (see [Converters](docs/converters.md)).
By default true.



<hr/>



<div class="method-overview">
<pre><code class="typescript-lang ">logger?<span class="token punctuation">:</span> Partial<<a href="#api/common/config/iloggersettings"><span class="token">ILoggerSettings</span></a>></code></pre>
</div>


Logger configuration.



<hr/>



<div class="method-overview">
<pre><code class="typescript-lang ">errors?<span class="token punctuation">:</span> Partial<<a href="#api/common/config/ierrorssettings"><span class="token">IErrorsSettings</span></a>></code></pre>
</div>


Errors configuration.



<hr/>



<div class="method-overview">
<pre><code class="typescript-lang ">controllerScope?<span class="token punctuation">:</span> <a href="#api/common/di/providerscope"><span class="token">ProviderScope</span></a></code></pre>
</div>


Configure the default scope of the controllers.

- Default: `singleton`. See [Scope](docs/scope.md).
- Values: `singleton`, `request`.



<hr/>



<div class="method-overview">
<pre><code class="typescript-lang ">routers?<span class="token punctuation">:</span> <a href="#api/common/config/iroutersettings"><span class="token">IRouterSettings</span></a></code></pre>
</div>


Global configuration for the Express.Router. See express [documentation](http://expressjs.com/en/api.html#express.router).



<hr/>



<div class="method-overview">
<pre><code class="typescript-lang "><span class="token punctuation">[</span>key<span class="token punctuation">:</span> <span class="token keyword">string</span><span class="token punctuation">]</span><span class="token punctuation">:</span> <span class="token keyword">any</span></code></pre>
</div>








