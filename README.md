# MIAGE-I2S-Advanced-Database


## Report build:

Use the **pdfLaTeX + PlantUML** recipe in VS Code, or run from this directory:

```sh
PLANTUML_JAR=/opt/homebrew/opt/plantuml/libexec/plantuml.jar latexmk -pdf -shell-escape -outdir=build report.tex
```

Edit `digrams/usecase/usecase.pu` to update the diagram.

The project includes the unmodified `plantuml.sty` version 0.7.0 from
https://mirrors.ctan.org/macros/luatex/latex/plantuml/plantuml.sty
(LPPL-1.3c+, Oliver Kopp and contributors). This version adds pdfLaTeX support
and `\plantumlinput`; the system-installed 0.6.0 lacks these features.
The local file takes precedence over the system package.
