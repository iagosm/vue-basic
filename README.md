# Vue3 - Basico

## DefineProps

- O defineProps é utilizado para definir as propriedades (props) que um componente pode receber. Ao chamar o componente, você pode passar valores para essas propriedades.

### Exemplo:

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML

### Dentro do componente, você pode definir as props usando o defineProps:

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`  </div><div class="slate-code_line">defineProps({</div><div class="slate-code_line">  msg: {</div><div class="slate-code_line">    type: String,</div><div class="slate-code_line">    required: true,</div><div class="slate-code_line">  },</div><div class="slate-code_line">})</div><div class="slate-code_line">  `

### Explicação:

- **msg**: Uma propriedade que deve ser do tipo String e é obrigatória para o funcionamento do componente.

## Components

- **Componente local**: Se o componente for usado dentro de outro componente, ele deve estar localizado na pasta /components.
- **Componente de rota**: Componente utilizado pelo roteamento, geralmente encontrado dentro da pasta views.
- **RouterView**: O RouterView é utilizado para carregar componentes de acordo com as rotas definidas.

## Composition API

- A Composition API é utilizada para criar a lógica do componente de forma mais flexível, especialmente para componentes mais complexos.

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML `</div><div class="slate-code_line">// Composition API</div><div class="slate-code_line">`

Dentro do , você pode definir propriedades, variáveis reativas, métodos e outros hooks que fazem parte da lógica do componente.</p><h2 class="slate-h2">Login Example (Event.prevent)</h2><ul class="slate-ul"><li class="slate-li"><div style="position:relative">O event.preventDefault() impede que o comportamento padrão de um evento aconteça, como enviar um formulário ou recarregar a página.</div></li></ul><h3 class="slate-h3">Exemplo:</h3><pre class="slate-code\_block"><select style="float:right" contenteditable="false"><option value="">Plain text</option><option value="antlr4">ANTLR4</option><option value="bash">Bash</option><option value="c">C</option><option value="csharp">C#</option><option value="css">CSS</option><option value="coffeescript">CoffeeScript</option><option value="cmake">CMake</option><option value="dart">Dart</option><option value="django">Django</option><option value="docker">Docker</option><option value="ejs">EJS</option><option value="erlang">Erlang</option><option value="git">Git</option><option value="go">Go</option><option value="graphql">GraphQL</option><option value="groovy">Groovy</option><option value="html">HTML</option><option value="java">Java</option><option value="javascript">JavaScript</option><option value="json">JSON</option><option value="jsx">JSX</option><option value="kotlin">Kotlin</option><option value="latex">LaTeX</option><option value="less">Less</option><option value="lua">Lua</option><option value="makefile">Makefile</option><option value="markdown">Markdown</option><option value="matlab">MATLAB</option><option value="markup">Markup</option><option value="objectivec">Objective-C</option><option value="perl">Perl</option><option value="php">PHP</option><option value="powershell">PowerShell</option><option value="properties">.properties</option><option value="protobuf">Protocol Buffers</option><option value="python">Python</option><option value="r">R</option><option value="ruby">Ruby</option><option value="sass">Sass (Sass)</option><option value="scss">Sass (Scss)</option><option value="scheme">Scheme</option><option value="sql">SQL</option><option value="shell">Shell</option><option value="swift">Swift</option><option value="svg">SVG</option><option value="tsx">TSX</option><option value="typescript">TypeScript</option><option value="wasm">WebAssembly</option><option value="yaml">YAML</option><option value="xml">XML</option></select><code ><div class="slate-code\_line"><form @submit.prevent="login"></div><div class="slate-code\_line"> <input type="text" placeholder="Email" v-model="email" /></div><div class="slate-code\_line"> <input type="text" placeholder="Password" v-model="password" /></div><div class="slate-code\_line"> <button type="submit">Login</button></div><div class="slate-code\_line"></form></div><div class="slate-code\_line"></div><div class="slate-code\_line"></div></code></pre><p class="slate-paragraph"><strong class="slate-bold">@submit.prevent="login"</strong>: Evita que o formulário seja enviado de forma tradicional, chamando a função login ao invés disso.</p><h2 class="slate-h2">V-model</h2><ul class="slate-ul"><li class="slate-li"><div style="position:relative">O v-model cria uma ligação bidirecional entre um campo de entrada e uma variável no Vue. Ou seja, sempre que o valor do input mudar, a variável também será atualizada, e vice-versa.</div></li></ul><pre class="slate-code\_block"><select style="float:right" contenteditable="false"><option value="">Plain text</option><option value="antlr4">ANTLR4</option><option value="bash">Bash</option><option value="c">C</option><option value="csharp">C#</option><option value="css">CSS</option><option value="coffeescript">CoffeeScript</option><option value="cmake">CMake</option><option value="dart">Dart</option><option value="django">Django</option><option value="docker">Docker</option><option value="ejs">EJS</option><option value="erlang">Erlang</option><option value="git">Git</option><option value="go">Go</option><option value="graphql">GraphQL</option><option value="groovy">Groovy</option><option value="html">HTML</option><option value="java">Java</option><option value="javascript">JavaScript</option><option value="json">JSON</option><option value="jsx">JSX</option><option value="kotlin">Kotlin</option><option value="latex">LaTeX</option><option value="less">Less</option><option value="lua">Lua</option><option value="makefile">Makefile</option><option value="markdown">Markdown</option><option value="matlab">MATLAB</option><option value="markup">Markup</option><option value="objectivec">Objective-C</option><option value="perl">Perl</option><option value="php">PHP</option><option value="powershell">PowerShell</option><option value="properties">.properties</option><option value="protobuf">Protocol Buffers</option><option value="python">Python</option><option value="r">R</option><option value="ruby">Ruby</option><option value="sass">Sass (Sass)</option><option value="scss">Sass (Scss)</option><option value="scheme">Scheme</option><option value="sql">SQL</option><option value="shell">Shell</option><option value="swift">Swift</option><option value="svg">SVG</option><option value="tsx">TSX</option><option value="typescript">TypeScript</option><option value="wasm">WebAssembly</option><option value="yaml">YAML</option><option value="xml">XML</option></select><code ><div class="slate-code\_line"><form @submit.prevent="login"></div><div class="slate-code\_line"> <input type="text" placeholder="Email" v-model="email" /></div><div class="slate-code\_line"> <input type="text" placeholder="Password" v-model="password" /></div><div class="slate-code\_line"> <button type="submit">Login</button></div><div class="slate-code\_line"></form></div><div class="slate-code\_line"></div><div class="slate-code\_line"></div></code></pre><p class="slate-paragraph"><strong class="slate-bold">v-model</strong>: Ligação do campo de entrada com a variável (no exemplo, email e password).</p><h2 class="slate-h2">Ref</h2><ul class="slate-ul"><li class="slate-li"><div style="position:relative">O ref é utilizado para criar referências reativas de tipos primitivos (string, número, etc.) no Vue 3. A referência se mantém atualizada automaticamente.</div></li></ul><h3 class="slate-h3">Exemplo:</h3><pre class="slate-code\_block"><select style="float:right" contenteditable="false"><option value="">Plain text</option><option value="antlr4">ANTLR4</option><option value="bash">Bash</option><option value="c">C</option><option value="csharp">C#</option><option value="css">CSS</option><option value="coffeescript">CoffeeScript</option><option value="cmake">CMake</option><option value="dart">Dart</option><option value="django">Django</option><option value="docker">Docker</option><option value="ejs">EJS</option><option value="erlang">Erlang</option><option value="git">Git</option><option value="go">Go</option><option value="graphql">GraphQL</option><option value="groovy">Groovy</option><option value="html">HTML</option><option value="java">Java</option><option value="javascript">JavaScript</option><option value="json">JSON</option><option value="jsx">JSX</option><option value="kotlin">Kotlin</option><option value="latex">LaTeX</option><option value="less">Less</option><option value="lua">Lua</option><option value="makefile">Makefile</option><option value="markdown">Markdown</option><option value="matlab">MATLAB</option><option value="markup">Markup</option><option value="objectivec">Objective-C</option><option value="perl">Perl</option><option value="php">PHP</option><option value="powershell">PowerShell</option><option value="properties">.properties</option><option value="protobuf">Protocol Buffers</option><option value="python">Python</option><option value="r">R</option><option value="ruby">Ruby</option><option value="sass">Sass (Sass)</option><option value="scss">Sass (Scss)</option><option value="scheme">Scheme</option><option value="sql">SQL</option><option value="shell">Shell</option><option value="swift">Swift</option><option value="svg">SVG</option><option value="tsx">TSX</option><option value="typescript">TypeScript</option><option value="wasm">WebAssembly</option><option value="yaml">YAML</option><option value="xml">XML</option></select><code ><div class="slate-code\_line"><script setup></div><div class="slate-code\_line">import { ref } from &#x27;vue&#x27;;</div><div class="slate-code\_line"></div><div class="slate-code\_line">const email = ref(&#x27;&#x27;);</div><div class="slate-code\_line">const password = ref(&#x27;&#x27;);</div><div class="slate-code\_line">

**ref** cria uma referência reativa para os dados do tipo primitivo.

## Reactive

- O reactive é semelhante ao ref, mas é utilizado para criar objetos reativos. Ele é perfeito para trabalhar com estruturas mais complexas, como objetos e arrays.

Exemplo:

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML `</div><div class="slate-code_line">import { reactive } from &#x27;vue&#x27;;</div><div class="slate-code_line"></div><div class="slate-code_line">const user = reactive({</div><div class="slate-code_line">  email: &#x27;&#x27;,</div><div class="slate-code_line">  password: &#x27;&#x27;</div><div class="slate-code_line">});</div><div class="slate-code_line">`

**reactive** cria um objeto reativo, permitindo que qualquer alteração em suas propriedades seja refletida automaticamente na interface.

## OnMounted

O onMounted é um hook da Composition API que é chamado assim que o componente é montado no DOM. Ele é ideal para carregar dados, fazer requisições API ou executar funções assim que o componente estiver pronto.

- Algo na hora que o component é carregado.
- Então sempre que o component for recarregado ou algo do tipo, irá mostrar o console abaixo
- Utilizado para requisições de API ou algo do tipo

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`  </div><div class="slate-code_line">import { onMounted } from &#x27;vue&#x27;;</div><div class="slate-code_line"></div><div class="slate-code_line">onMounted(() => {</div><div class="slate-code_line">  console.log(&#x27;Componente montado&#x27;);</div><div class="slate-code_line">});</div><div class="slate-code_line">  `

O **console.log** será exibido assim que o componente for montado.

## V-if

- O v-if é usado para renderizar condicionalmente um elemento ou componente. Ele só será exibido se a condição for verdadeira.

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`  </div><div class="slate-code_line">import { reactive } from &#x27;vue&#x27;;</div><div class="slate-code_line"></div><div class="slate-code_line">const user = reactive({</div><div class="slate-code_line">  email: &#x27;&#x27;,</div><div class="slate-code_line">  password: &#x27;&#x27;</div><div class="slate-code_line">});</div><div class="slate-code_line">  `

O elemento div será exibido apenas quando o email for vazio.

## **V-else**

O v-else é utilizado para criar uma alternativa ao v-if. Ele só será renderizado se a condição do v-if não for satisfeita.

Exemplo:

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML

## Instalar Tailwind CSS

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`  npm install tailwindcss @tailwindcss/vite  import { defineConfig } from 'vite';  import vue from '@vitejs/plugin-vue';  import tailwindcss from 'tailwindcss';  //   export default defineConfig({    plugins: [vue()],    css: {      postcss: {        plugins: [tailwindcss],      },    },  });  `
