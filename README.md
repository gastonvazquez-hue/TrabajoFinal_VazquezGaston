# Predicción de la Informalidad Laboral en Argentina

Trabajo final para el **Curso de Posgrado en Ciencia de Datos** (Universidad Nacional del Comahue — Facultad de Economía y Administración, Departamento de Estadística).

Este proyecto desarrolla un modelo predictivo supervisado de clasificación binaria (Regresión Logística) para estimar la probabilidad de informalidad laboral en trabajadores asalariados de Argentina. Utiliza los microdatos de la Encuesta Permanente de Hogares (EPH - INDEC) del primer trimestre de 2026 y se implementa dentro del ecosistema `tidymodels` en R.

---

## 📁 Estructura del Repositorio

* **`TrabajoFinal_VazquezGaston.Rproj`**: Archivo de proyecto de RStudio para la gestión automática del directorio de trabajo y rutas relativas.
* **`TrabajoFinal_VazquezGaston.qmd`**: Documento principal en Quarto con el flujo de trabajo completo (EDA, preprocesamiento, modelado y métricas).
* **`Informe Final Curso de Posgrado_VazquezGaston.pdf`**: Reporte técnico final compilado.
* **`Header_TrabajoFinal.tex`**: Configuración de formato y estilos LaTeX para la exportación a PDF.
* **`References_TrabajoFinal.bib`**: Archivo de referencias bibliográficas en formato BibTeX.
* **`Figuras/`**: Gráficos generados durante el análisis (Curva ROC, Matriz de Confusión).

---

## 🛠️ Requisitos e Instalación

Para ejecutar y reproducir el proyecto se requiere **R** y el CLI de **Quarto**. Los paquetes principales de R utilizados son:

```r
install.packages(c(
  "tidyverse", 
  "tidymodels", 
  "eph", 
  "gt", 
  "skimr", 
  "psych", 
  "yardstick"
))
