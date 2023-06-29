# Visual Studio Code

{% code title=".vscode/task.json" %}
```json
{
  "version": "...",
  "tasks": [
    {
      "type": "cppbuild",
      "label": "...",
      "command": "...",
      "args": [
        "-fdiagnostics-color=always",
        "-g",
        "${workspaceFolder}\\src\\*.cpp",
        "${workspaceFolder}\\src\\include\\StyioUtil\\*.cpp",
        "${workspaceFolder}\\src\\include\\StyioParser\\*.cpp",
        "-o",
        "${fileDirname}\\${fileBasenameNoExtension}.exe"
        ],
        "options": {}
  ]
}
```
{% endcode %}

```
"-g",
"${workspaceFolder}\\src\\*.cpp",
"${workspaceFolder}\\src\\include\\StyioUtil\\*.cpp",
"${workspaceFolder}\\src\\include\\StyioParser\\*.cpp",
```

