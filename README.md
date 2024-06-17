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
<h2>Configurar o visual studio</h2>
<p>Abaixar algumas extensões no visual studio</p>
<ul>
      <li>ESlint</li>
      <li>Prettier - Code formatter</li>
</ul>
<p>Coloca seguinte comando no arquivo json do <strong>visual studio</strong>(pro eslint poder corrigir os arquivos)</p>

comando: 
<pre>
<code>
"editor.codeActionsOnSave": {
      "source.fixAll.eslint": "explicit",
      "source.fixAll": "explicit"
}
</code>
</pre>

# Correção
Voce so precisa <strong> npm i -D eslint-config-prettier eslint-config-airbnb eslint-plugin-import</strong> e oa rquivo prettier

# Para o vite
tem que abaixar <strong>npm i -D eslint-config-prettier eslint-config-airbnb</strong> criar arquivo json <strong>.prettierrc</strong> e adiciona airbnb e prettier no extends<br>
Opcional colocar <strong>react-hooks</strong> em plugins


