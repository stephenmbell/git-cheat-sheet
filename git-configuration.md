
# basic git configuration

`# tell git who you are`

git config --global user.name "Firstname Lastname"

`# tell git how to email you`

git config --global user.email "myemail@domain.com"

`# handles end of line character differences between windows and linux`

git config --global core.autocrlf true

`# prevents conversion warning messages`

git config --global core.safecrlf

`# set default git editor`

git config --global core.editor "~\path\to\editor.exe"
`# path to vscode`

"~\AppData\Local\Programs\Microsoft VS Code\Code.exe"

`# list current git configuration`

git config --list
