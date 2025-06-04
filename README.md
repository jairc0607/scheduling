# 🧠 GeneticSchoolScheduler - Horarios Escolares con Algoritmos Genéticos

Este repositorio contiene el desarrollo completo del modelo de optimización de horarios escolares para la **Unidad Educativa Lev Vygotsky**, como parte del proyecto de titulación de la **Maestría en Ciencia de Datos**. Se implementa un algoritmo genético híbrido capaz de generar horarios viables, respetando múltiples restricciones duras y blandas propias del contexto educativo real.

## 🎯 Objetivo del Proyecto

Optimizar la asignación semanal de clases para 48 paralelos escolares (de 1EGB a 3BGU), considerando:
- Restricciones duras (recesos, continuidad, cruce docente, franjas de especialidad).
- Restricciones blandas (licencias de maternidad, medio tiempo).
- Criterios pedagógicos y operativos definidos por la institución.

El modelo se basa en la representación cromosómica de asignaciones y aplica operadores genéticos especializados para preservar la factibilidad.

---

## 📁 Estructura del Repositorio

| Notebook | Descripción |
|----------|-------------|
| `main.ipynb` | Implementación principal del algoritmo genético, incluyendo evaluación, selección, cruces y mutación. |
| `Cromosoma_LEV.ipynb` | Construcción del cromosoma base a partir del horario vigente del colegio. |
| `IMG_a_CSV.ipynb` | Conversión automática de horarios en imágenes a archivos `.txt` estructurados (OCR y formateo). |
| `Visualización_Horario.ipynb` | Generación de tablas en LaTeX para visualizar el horario de cada curso. |
| `Pueba_función_fitness.ipynb` | Evaluación y validación de la función fitness sobre el horario actual. |

---

## ⚙️ Tecnologías y Entorno

- **Lenguaje**: Python 3.10+
- **Entorno de trabajo**: Google Colab Pro+
- **Formato cromosoma**: Lista de tuplas con estructura:
  ```python
  (nivel, aula, día, hora, materia, docente)
