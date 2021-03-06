
<header class="symbol-info-header"><h1 id="broadcast">Broadcast</h1><label class="symbol-info-type-label decorator">Decorator</label></header>
<!-- summary -->
<section class="symbol-info"><table class="is-full-width"><tbody><tr><th>Module</th><td><div class="lang-typescript"><span class="token keyword">import</span> { Broadcast }&nbsp;<span class="token keyword">from</span>&nbsp;<span class="token string">"@tsed/socketio"</span></div></td></tr><tr><th>Source</th><td><a href="https://github.com/Romakita/ts-express-decorators/blob/v4.23.1/src//socketio/decorators/broadcast.ts#L0-L0">/socketio/decorators/broadcast.ts</a></td></tr></tbody></table></section>
<!-- overview -->


### Overview


<pre><code class="typescript-lang ">function <span class="token function">Broadcast</span><span class="token punctuation">(</span>eventName<span class="token punctuation">:</span> <span class="token keyword">string</span><span class="token punctuation">)</span><span class="token punctuation">:</span> <span class="token punctuation">(</span>target<span class="token punctuation">:</span> <span class="token keyword">any</span><span class="token punctuation">,</span> propertyKey<span class="token punctuation">:</span> <span class="token keyword">string</span><span class="token punctuation">,</span> descriptor<span class="token punctuation">:</span> PropertyDescriptor<span class="token punctuation">)</span> => <span class="token keyword">void</span><span class="token punctuation">;</span></code></pre>


<!-- Parameters -->

<!-- Description -->


### Description

Broadcast the response for all client registered in the same namespace.

With the `@Broadcast` decorator, the method will accept a return type (Promise or not).

### Example

```typescript
@SocketService("/nsp")
export class MyWS {

  @Input("event")
  @Broadcast("returnEvent")
  async myMethod(@Args(0) data: any, @Nsp socket): Promise<any> {
     return Promise.resolve({data})
  }
}
```

<!-- Members -->

