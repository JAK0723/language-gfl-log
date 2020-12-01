# GFL Log language package

Syntax highlighting for Girls' Frontline logs.

To enable automatic syntax highlighting, add the following to `init.coffee`, replacing `<PATH>` with the path to your log directory:

```coffeescript
atom.workspace.observeTextEditors (editor) ->
  if editor.getPath().includes('<PATH>')
    editor.setGrammar(atom.grammars.grammarForScopeName('source.gfl-log'))
```
