# FORM-IC-01: arquitecturas distribuidas en la industria

Investigación individual de Aplicaciones Distribuidas (ISR-701), UTEQ, paralelo B.

- **Estudiante:** Benites Pérez Dariem Alberto
- **Caso:** Uber y su arquitectura de microservicios orientada a dominios (DOMA)
- **Fuente principal:** A. Gluck, [*Introducing Domain-Oriented Microservice Architecture*](https://www.uber.com/blog/microservice-architecture/), Uber Engineering Blog, 23 de julio de 2020.

## Contenido

| Carpeta o archivo | Qué tiene |
|---|---|
| [`documento/main.tex`](documento/main.tex) | El análisis de una página, las evidencias y la declaración de IA |
| [`documento/main.pdf`](documento/main.pdf) | El PDF compilado |
| [`documento/referencias.bib`](documento/referencias.bib) | Las referencias en formato IEEE (biblatex) |
| [`capturas/`](capturas/) | La captura de la fuente con mis subrayados |
| [`caratula/`](caratula/) | La carátula de una página que se sube al SGA |

## Cómo compilar

- **Compilador:** `pdflatex`, con `biber` para las referencias.
- **Archivo principal:** `documento/main.tex`.
- **Dependencias:** una distribución de LaTeX (MiKTeX o TeX Live) con `biblatex`, `biblatex-ieee`, `babel` (español), `csquotes`, `tabularx`, `xcolor`, `hyperref` y `xurl`.

Desde la carpeta `documento`:

```
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
```

La carátula se compila con una sola pasada de `pdflatex caratula.tex` dentro de `caratula`.
