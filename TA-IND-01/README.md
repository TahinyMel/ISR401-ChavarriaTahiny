# TA-IND-01 — Análisis de requisitos de PayPal

**Asignatura:** Ingeniería de Requerimientos (ISR-401) — UTEQ.  
**Estudiante:** Chavarria Cuenca Tahiny Mel  
**Actividad:** TA-IND-01 — IEEE 29148 y tipos de requisitos de un sistema conocido.  
**Repositorio:** https://github.com/TahinyMel/ISR401-ChavarriaTahiny/tree/main/TA-IND-01

## Estructura

- `main.tex`: informe principal, 10 entradas de glosario, 15 requisitos, tabla, análisis, autoevaluación, reflexión y declaración de IA.
- `referencias.bib`: bibliografía cotejada con fuentes verificables; estilo IEEE.
- `main.pdf`: versión compilada del informe.
- `figuras/`: carpeta para capturas.


## Compilación reproducible

**Motor:** pdfLaTeX. **Bibliografía:** Biber, estilo `biblatex-ieee`.  
**Dependencias:** TeX Live completo o MiKTeX actualizado con `extarticle`, `babel` para español, `geometry`, `lmodern`, `microtype`, `graphicx`, `booktabs`, `longtable`, `tabularx`, `caption`, `subcaption`, `titlesec`, `fancyhdr`, `lastpage`, `biblatex`, `biber`, `hyperref`.

Desde `TA-IND-01/`, ejecutar en este orden:

```sh
pdflatex -interaction=nonstopmode -halt-on-error main.tex
biber main
pdflatex -interaction=nonstopmode -halt-on-error main.tex
pdflatex -interaction=nonstopmode -halt-on-error main.tex
pdflatex -interaction=nonstopmode -halt-on-error entrega_sga.tex
pdflatex -interaction=nonstopmode -halt-on-error entrega_sga.tex
```

Alternativa: `latexmk -pdf -interaction=nonstopmode main.tex` (con `biber` instalado). En Overleaf, elegir pdfLaTeX y compilación con Biber. Atención: esta actividad emplea **Biber**, no `bibtex`, a diferencia del README del ejercicio anterior `FORM-TL-01`.


## Fuentes

ISO/IEC/IEEE 29148:2018 (norma), ISO/IEC 25010:2023 (modelo de calidad), Pohl (2025), SWEBOK v4.0 (2024), y páginas oficiales de PayPal. Referencias concretas en `referencias.bib`.

