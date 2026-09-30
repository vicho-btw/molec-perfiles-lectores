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
| `Etapa1.Rmd` | Reporte de la Etapa 1 (código + texto). |
| `Etapa1.pdf` | Reporte compilado (borrador). |
| `DatosEquipo_MOLEC_2019_2024.csv` | Base de trabajo limpia: 10,252 registros, 25 variables. La genera `Etapa1.Rmd`. |
| `datos/` | Microdatos y diccionarios de MOLEC 2019–2025 tal como los publica INEGI. |
| `plantilla_word.docx` | Estilos para la salida en Word (interlineado 1.5). |
| `img/logo_tec.png` | Logo para la portada del PDF (curso y profesor van en el YAML de `Etapa1.Rmd`). |

## Cómo compilar

1. Abrir `situacionproblema.Rproj` en RStudio.
2. Instalar paquetes si hace falta: `install.packages(c("dplyr", "tidyr", "ggplot2", "knitr", "readxl", "rmarkdown"))`.
3. Abrir `Etapa1.Rmd` → **Knit → Knit to PDF** (requiere LaTeX; con `tinytex::install_tinytex()` basta).

## Fuente de los datos

INEGI. *Módulo sobre Lectura (MOLEC)*. https://www.inegi.org.mx/programas/molec/
