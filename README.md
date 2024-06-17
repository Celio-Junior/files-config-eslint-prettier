<h1>Eslint para o <strong>React</strong></h1>
<h2>Instações de pacotes necessarios(jeito antigo)<h2>

<p>
      1 - abaixa os pacotes com devDepencências(npm i -D ou <strong>npm i --save-dev</strong>):
      <ul>
            <li>@babel/eslint-plugin</li>
            <li>@babel/preset-react</li>
            <li>eslint-config-prettier</li>
            <li>eslint-plugin-prettier</li>
            <li>prettier</li>
      </ul>
      Ou:
</p>

<pre>
<code>
      npm i -D @babel/eslint-plugin @babel/preset-react eslint-config-prettier eslint-plugin-prettier prettier
</code>
</pre>

<p>
      2 - depois colocar os arquivos: <strong>.babelrc.json e .prettierrc.js </strong> na raiz ou na pasta src(ou algo parecido) no seu projeto
</p>
<h2>3 - Configurar o visual studio</h2>
<p>Abaixar algumas extensões no visual studio</p>
<ul>
      <li>ESlint</li>
      <li>Prettier - Code formatter(antes não presisava mais atualmente é melhor usar)</li>
</ul>
<p>Inseri o seguinte comando no arquivo json do seu <strong>visual studio</strong>(pro eslint tentar corrigir os arquivos):</p>

<pre>
<code>
"editor.codeActionsOnSave": {
      "source.fixAll.eslint": "explicit",
      "source.fixAll": "explicit"
}
</code>
</pre>

<p>Tambem inseri esse comando no arquivo json do visual studio(esse pra que vs usar o prettier como formatador do código):</p>

<pre>
<code>
"editor.defaultFormatter": "esbenp.prettier-vscode",
  "[javascript]": {
    // "editor.formatOnSave": true,
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "editor.formatOnSave": true
</code>
</pre>

<h2>Correção</h2>
<p>Observação: <em> usa as configurações do visual studio que foi citado(recomendo, pois se não vai dar certo)</em></p>
<p>
      Voce so precisa agora atualmente usa só os comandos <strong> npm i -D eslint-config-prettier eslint-config-airbnb</strong> e o arquivo <strong>.prettierrc.js(como exemplo do 
      arquivo do repositorio</strong> <br>
      e colocar no arquivo .eslint.js(se tu usando <strong>npx create-react-app</strong>) ou  e nesse arquivo dentro da chave extends colocar em ultimo(tem que ser em ultimo):
</p>

<pre>
<code>
extends: [
  'airbnb',
  'prettier',
]
</code>
</pre>
<p>
      também eu recomendo colocar dentro do arquivo em eslint na chave em plugins(se não tiver tem o arquivo acima como referência):
</p>

<pre>
<code>
plugins: ["react", "react-hooks"]
</code>
</pre>

<h2>Para o vite</h2>
<p>
      Tem que abaixar <strong>npm i -D eslint-config-prettier eslint-config-airbnb</strong> criar arquivo json <strong>.prettierrc(não precisa colocar extensão json)</strong><br>
      e adiciona airbnb e prettier no extends, Opcional colocar <strong>react-hooks</strong> em plugins
</p>

<p>Vê arquivo .eslintrc.cjs dentro da pasta new_arquivo nesse diretorio para vê como referência ou copiar, sente-se a vontade de usar</p>


