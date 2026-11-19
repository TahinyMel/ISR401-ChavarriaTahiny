# EV-PRAC-01 · Compilación del PDF

Necesitas una distribución de LaTeX con `pdflatex`, como MiKTeX o TeX Live.

Abre una terminal en la carpeta que contiene `EVPractica.tex` y ejecuta ambos comandos:

```sh
pdflatex -halt-on-error -jobname=EV_Practica EVPractica.tex
pdflatex -halt-on-error -jobname=EV_Practica EVPractica.tex
```

La segunda pasada actualiza las referencias de página. El archivo `EV_Practica.pdf` se genera en la misma carpeta.

