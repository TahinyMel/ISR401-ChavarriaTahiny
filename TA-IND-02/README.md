# TA-IND-02 · Priorización de requisitos

Trabajo individual de Ingeniería de Requerimientos (ISR-401), UTEQ. El informe compara MoSCoW, Kano y votación ponderada.

## Compilación del informe

- **Archivo principal** — `TA-IND-02/main.tex`.
- **PDF generado** — `TA-IND-02/main.pdf`.
- **Compilador** — pdfLaTeX, incluido en TeX Live o MiKTeX.
- **Bibliografía** — BibTeX. El siguiente procedimiento supone que `main.tex` usa `\bibliographystyle{IEEEtran}` y `\bibliography{referencias}`,
- con el archivo `TA-IND-02/referencias.bib`.
- **Dependencias** — Git para clonar, el estilo bibliográfico `IEEEtran.bst`, los paquetes que cargue `main.tex` y los archivos locales que incluya el informe, como figuras y secciones. Una instalación completa de TeX Live simplifica la instalación de paquetes. Si usas MiKTeX, instala los paquetes que falten desde MiKTeX Console.

1. Clona el repositorio público y entra en la carpeta del informe. 

```sh
   git clone https://github.com/TahinyMel/ISR401-ChavarriaTahiny.git
   cd ISR401-ChavarriaTahiny/TA-IND-02
   ```

2. Ejecuta estos comandos en orden y corrige cualquier error antes de pasar al siguiente.

   ```sh
   pdflatex -interaction=nonstopmode -halt-on-error main.tex
   bibtex main
   pdflatex -interaction=nonstopmode -halt-on-error main.tex
   pdflatex -interaction=nonstopmode -halt-on-error main.tex
   ```

3. Abre `main.pdf` y comprueba que se vean las figuras, las tablas y la bibliografía, y que no aparezcan citas ni referencias sin resolver (`?` o `??`). El PDF compilado se entrega en el repositorio junto con los fuentes.
