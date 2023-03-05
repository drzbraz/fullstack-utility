### Linux
O comando "mv" tem a função de mover arquivos. A utilização dele é praticamente igual  a do comando cp. Exemplo:
$ mv MV.txt /home/baixaki/Trabalho/MV.txt  - O arquivo MV.txt foi movido para a pasta /home/baixaki/Trabalho com o mesmo nome.
$ mv MV.txt  VM.txt – O arquivo MV.txt continuou onde estava, porém, agora possui o nome de VM.txt.

sudo apt-get install -f : Para instalar todas as dependencias do pacote

Para renomear arquivos: mv (nome do arquivo atual) (nome do arquivo que deseja)

/etc/apt/sources.list.d/
tar -vzxf nomedoarquivo


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


git reset --hard

### Default configuration VSCODE

{
  "terminal.integrated.fontSize": 14,
  "workbench.iconTheme": "material-icon-theme",
  "workbench.startupEditor": "newUntitledFile",
  "editor.tabSize": 2,
  "editor.fontSize": 18,
  "editor.lineHeight": 26,
  "editor.fontFamily": "Fira Code",
  "editor.fontLigatures": true,
  "explorer.compactFolders": false,
  "editor.renderLineHighlight": "gutter",
  "workbench.editor.labelFormat": "short",
  "extensions.ignoreRecommendations": true,
  "javascript.updateImportsOnFileMove.enabled": "always",
  "typescript.updateImportsOnFileMove.enabled": "never",
  "breadcrumbs.enabled": true,
  "editor.parameterHints.enabled": false,
  "explorer.confirmDragAndDrop": false,
  "explorer.confirmDelete": false,
  "editor.rulers": [
    80,
    120
  ],
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  },
  "files.associations": {
    ".sequelizerc": "javascript",
    ".stylelintrc": "json",
    ".prettierrc": "json"
  },
  "window.zoomLevel": 0,
  "emmet.syntaxProfiles": {
    "javascript": "jsx"
  },
  "emmet.includeLanguages": {
    "javascript": "javascriptreact",
    "njk": "html"
  },
  "gitlens.codeLens.recentChange.enabled": false,
  "gitlens.codeLens.authors.enabled": false,
  "gitlens.codeLens.enabled": false,
  "git.enableSmartCommit": true,
  "terminal.integrated.shell.osx": "/bin/zsh",
  "liveshare.featureSet": "insiders",
  "typescript.tsserver.log": "verbose",
  "javascript.suggest.autoImports": true,
  "typescript.suggest.autoImports": true,
  "javascript.preferences.quoteStyle": "single",
  "typescript.preferences.quoteStyle": "single",
  "prettier.jsxSingleQuote": true,
  "prettier.singleQuote": true,
  "liveServer.settings.donotShowInfoMsg": true,
  "material-icon-theme.activeIconPack": "nest",
  "screencastMode.onlyKeyboardShortcuts": true,
  "material-icon-theme.folders.associations": {
    "infra": "app",
    "entities": "class",
    "schemas": "class",
    "typeorm": "database",
    "repositories": "mappings",
    "http": "container",
    "migrations": "tools",
    "modules": "components",
    "implementations": "core",
    "dtos": "typescript",
    "fakes": "mock",
    "websockets": "pipe",
    "protos": "pipe",
    "grpc": "pipe"
  },
  "material-icon-theme.files.associations": {
    "ormconfig.json": "database",
    "tsconfig.json": "tune",
    "*.proto": "3d"
  },
  "workbench.colorTheme": "Dracula",
  "editor.formatOnType": true
}

# Default configuration global css:
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}




body,
input,
textarea,
select,
button {
  font: 400 1rem 'Roboto', sans-serif;
}

@media (max-width: 1080px) {
  //tablet
  html {
    font-size: 93.75%; //15px
  }
}

@media (max-width: 720px) {
  //mobile
  html {
    font-size: 87.5%; //14px
  }
}

button {
  cursor: pointer;
}

a {
  color: inherit;
  text-decoration: none;
}

