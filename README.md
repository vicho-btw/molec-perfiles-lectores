# La realidad de la lectura en México: perfiles lectores y su evolución (MOLEC 2019–2024)

Reto de Estadística: análisis del Módulo sobre Lectura (MOLEC) del INEGI.

**Pregunta de investigación.** ¿Qué perfiles de lector existen en la población urbana mexicana de 18 años y más, según su comportamiento lector reportado en MOLEC 2019–2024, y cómo ha cambiado el peso de cada perfil a lo largo de esos años?

**Método (planeado).** *k-means* sobre variables de comportamiento lector, validación con variables externas (edad, escolaridad, sexo, entidad, antecedentes de lectura en hogar y escuela) y análisis de la tendencia de cada perfil por año con el factor de expansión.

## Equipo

- Vicente Alonso Gallardo Montalva 
- Jia-Hong André Kuo Ko 
- Mauricio Ruiz Junco
- Mauricio Orcasitas Fara

## Contenido

| Archivo | Descripción |
|---|---|
| `ReporteFinal.Rmd` | Reporte final (código + texto): preparación de datos, análisis descriptivo, inferencia, arquetipos con k-means y estrategia de fomento. |
| `ReporteFinal.pdf` | Reporte final compilado. |
| `Presentacion.pptx` | Presentación para la exposición (PowerPoint; se puede abrir en Google Slides). |
| `Presentacion.pdf` | Presentación en PDF. |
| `BasePreparada_MOLEC_2019_2024.csv` | Base preparada: 11,685 personas alfabetas, 32 variables, con la partición entrenamiento/validación/prueba. La genera `ReporteFinal.Rmd`. |
| `BasePerfiles_MOLEC_2019_2024.csv` | Base preparada con la columna `perfil` (6 arquetipos de k-means). La genera `ReporteFinal.Rmd`. |
| `datos/` | Microdatos y diccionarios de MOLEC 2019–2025 tal como los publica INEGI. |
| `img/logo_tec.png` | Logo para la portada del PDF. |

Las versiones entregadas de cada etapa están en el historial de git.

## Cómo compilar

1. Abrir `situacionproblema.Rproj` en RStudio.
2. Instalar paquetes si hace falta: `install.packages(c("dplyr", "tidyr", "ggplot2", "knitr", "readxl", "rmarkdown", "kableExtra", "e1071", "gridExtra", "cluster", "car"))`.
3. Abrir `ReporteFinal.Rmd` → **Knit → Knit to PDF** (requiere LaTeX; con `tinytex::install_tinytex()` basta).

## Fuente de los datos

INEGI. *Módulo sobre Lectura (MOLEC)*. https://www.inegi.org.mx/programas/molec/
