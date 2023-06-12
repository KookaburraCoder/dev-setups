# Visual Studio Code & Ruby on Rails

### Extensions

Just to expand, I use prettier for my formatting, as well as ERB formatter. Error lens shows me errors on the file as opposed to the problems panel.

- Prettier - Code formatter [Marketplace Link](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
- ERB Formatter/Beautify [Marketplace Link](https://marketplace.visualstudio.com/items?itemName=aliariff.vscode-erb-beautify)
- Error Lens [Marketplace Link](https://marketplace.visualstudio.com/items?itemName=usernamehw.errorlens)
- Ruby [Marketplace Link](https://marketplace.visualstudio.com/items?itemName=rebornix.Ruby)
- VSCode Ruby [Marketplace Link](https://marketplace.visualstudio.com/items?itemName=wingrunr21.vscode-ruby)
- IntelliCode [Marketplace Link](https://marketplace.visualstudio.com/items?itemName=VisualStudioExptTeam.vscodeintellicode)

### Gems

These gems will be needed for prettier to format ruby files.

- bundler
- prettier_print
- syntax_tree
- syntax_tree-haml
- syntax_tree-rbs

Command

```bash
gem install bundler prettier_print syntax_tree syntax_tree-haml syntax_tree-rbs
```

### settings.json

This will setup prettier as the formatter for ruby, and set the formatter for erb files.

```json
"[ruby]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode",
    "editor.formatOnSave": true
},
"[erb]": {
    "editor.defaultFormatter": "aliariff.vscode-erb-beautify",
    "editor.formatOnSave": true
},
"files.associations": {
    "*.html.erb": "erb"
},
```
