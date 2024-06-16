# Instações de pacotes necessarios

abaixa os pacotes com devDepencências(npm i -D):
- @babel/eslint-plugin
- @babel/preset-react
- eslint-config-prettier
- eslint-plugin-prettier
- prettier
Ou <strong>- npm i -D @babel/eslint-plugin @babel/preset-react eslint-config-prettier eslint-plugin-prettier prettier</strong> <br>
depois colocar os arquivos: <strong>.babelrc.json e ,prettierrc.js </strong>

# Configurar o visual studio
Coloca seguinte comando no arquivo json do vs(pro eslint poder corrigir os arquivos)

comando: 
<code>
"editor.codeActionsOnSave": {
      "source.fixAll.eslint": "explicit",
      "source.fixAll": "explicit"
}
</code>

# Correção
Voce so precisa <strong> npm i -D eslint-config-prettier eslint-config-airbnb eslint-config-prettier eslint-plugin-import</strong> e oa rquivo prettier
