# Latex Repo
For CVs and stuff

For Ubuntu and Mate:
```shellscript
sudo add-apt-repository ppa:jonathonf/texlive
sudo apt update && sudo apt install texlive-full
```

VS Code Extension:
LaTeX Workshop

## Setup LuaTeX and Biber in settings.json
```
 "latex-workshop.latex.recipes": [
        {
            "name": "lualatex->biber->lualatex",
            "tools": [
                "lualatex",
                "biber",
                "lualatex"
            ]
        }
    ],
    "latex-workshop.latex.tools": [
        {
            "name": "lualatex",
            "command": "lualatex",
            "args": [
                "-synctex=1",
                "-interaction=nonstopmode",
                "-file-line-error",
                "-pdf",
                "%DOC%"
            ]
        },
        {
            "name": "biber",
            "command": "biber",
            "args": [
                "%DOCFILE%"
            ]
        }
    ]
 ```
