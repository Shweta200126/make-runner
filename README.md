## Makefile Runner
Allows us to run/copy make targets directly from vscode terminal.
### Setup Options(Optional)
To export environment variables while running targets.
Open `settings.json` and add configs
``` json
"make-runner.env": {
  "development": {
    "AWS_PROFILE": "development",
    "RAILS_ENV": "development",
    "ROLE": "admin",
    "ENABLE_MFA": false
  },
  "staging": {
    "AWS_PROFILE": "staging",
    "RAILS_ENV": "staging",
    "ROLE": "user",
    "ENABLE_MFA": true
  },
  "none": {}
}
```
<b>Note</b>: This is optional step to export environment variables while running targets.

### Usage
Open any Makefile
Put the cursor on any target
- Use key bindings `cmd+shift+enter` for Mac or `ctrl+shift+enter` for PC to run the target
- Use key bindings `cmd+shift+c` for Mac or `ctrl+shift+c` for PC to copy the target command
![](sample.gif)
