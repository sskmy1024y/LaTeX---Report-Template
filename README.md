# LaTeX Report Template
This template is for university reports.

## How to use
Clone this repository and edit `main.tex`.

## notebook for me
Auto compile with VSCode. 
Install `LaTeX Workshop` and write settings.

```json
"latex-workshop.latex.tools": [
    {
        "name": "ptex2pdf",
        "command": "ptex2pdf",
        "args": [
            "-l",
            "-ot",
            "-kanji=utf8 -synctex=1 -interaction=nonstopmode -shell-escape",
            "%DOCFILE%.tex"
        ]
    },
],
"latex-workshop.latex.recipes": [
    {
        "name": "ptex2pdf",
        "tools": [
            "ptex2pdf",
            "ptex2pdf"
        ]
    }
],
"latex-workshop.latex.clean.enabled": true,
"latex-workshop.view.pdf.viewer": "tab",
"latex-workshop.chktex.enabled": false,
```