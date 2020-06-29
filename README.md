### Linux
O comando "mv" tem a função de mover arquivos. A utilização dele é praticamente igual  a do comando cp. Exemplo:
$ mv MV.txt /home/baixaki/Trabalho/MV.txt  - O arquivo MV.txt foi movido para a pasta /home/baixaki/Trabalho com o mesmo nome.
$ mv MV.txt  VM.txt – O arquivo MV.txt continuou onde estava, porém, agora possui o nome de VM.txt.

sudo apt-get install -f : Para instalar todas as dependencias do pacote

Para renomear arquivos: mv (nome do arquivo atual) (nome do arquivo que deseja)

/etc/apt/sources.list.d/



### Docker
docker ps : mostrar containers ativas
docker ps -a : mostrar todas as containers
docker start (id container): iniciar uma containers
docker stop (id container): parar uma containers

### MongoDB

Para filtrar um range de datas:

db.getCollection('nome da collection').find({ 
    "createdAt": {
        $gte: ISODate("2020-04-06T00:00:00.000-03:00"),
        $lt: ISODate("2020-04-22T23:59:59.999-03:00")
    }
})

### Default configuration VSCODE

{
  "workbench.iconTheme": "material-icon-theme",
  "workbench.colorTheme": "Dracula",
  "window.zoomLevel": 0,
  "javascript.updateImportsOnFileMove.enabled": "always",
  "editor.fontFamily": "Fire Code",
  "editor.fontLigatures": true,
  "terminal.integrated.fontFamily": "monospace",
  "editor.fontSize": 18,
  "editor.lineHeight": 24,
  "editor.formatOnSave": true,
  "editor.rulers": [80, 120],
  "editor.tabSize": 2,
  "editor.renderLineHighlight": "gutter",
  "terminal.integrated.fontSize": 14,
  "emmet.syntaxProfiles": {
    "javascript": "jsx"
  },
  "emmet.includeLanguages": {
    "javascript": "javascriptreact",
    "njk": "html"
  },
  "breadcrumbs.enabled": true,
  "editor.parameterHints.enabled": false,
  "javascript.preferences.quoteStyle": "single",
  "typescript.preferences.quoteStyle": "single",
  "[javascript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "prettier.jsxSingleQuote": true,
  "prettier.singleQuote": true,
  "javascript.format.insertSpaceAfterSemicolonInForStatements": false,
  "prettier.semi": false,
  "typescript.format.insertSpaceAfterSemicolonInForStatements": false,
  "liveServer.settings.donotShowInfoMsg": true
}
