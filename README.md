# Minimal Reconnection for Brain Resilience: A Strategic Reconnection Framework (ORT-THERAPY-F) for Damaged Connectomes

[![Autor](https://img.shields.io/badge/Autor-Jos%C3%A9%20Ignacio%20Peinador%20Sala-lightgrey.svg)](https://orcid.org/0009-0008-1822-3452)
[![ORCID](https://img.shields.io/badge/ORCID-0009--0008--1822--3452-A6CE39.svg?logo=orcid&logoColor=white)](https://orcid.org/0009-0008-1822-3452)
[![Contacto](https://img.shields.io/badge/Contacto-joseignacio.peinador@gmail.com-007BFF.svg)](mailto:joseignacio.peinador@gmail.com)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)
[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.17417142.svg)](https://doi.org/10.5281/zenodo.17417142)

---

![Ilustración conceptual de ORT-THERAPY-F](httpsEntry_Image.jpg)
*Ilustración conceptual que muestra la "Absorción por Componente Gigante" (GCA). La intervención mínima de ORT-THERAPY-F reconecta el conectoma dañado y fragmentado (izquierda) para restaurar su integridad topológica (derecha).*

---

Este repositorio contiene el código, los datos y los experimentos del artículo de investigación "**Minimal Reconnection for Brain Resilience: A Strategic Reconnection Framework (ORT-THERAPY-F) for Damaged Connectomes**".

El proyecto modela la fragmentación progresiva en enfermedades neurodegenerativas (como el Alzheimer) como un **ataque dirigido que prioriza la vulnerabilidad de los 'hubs' (nodos de alta conectividad)**.

Proponemos ORT-THERAPY-F, un framework computacional que valida una heurística de reconexión estratégica llamada **'Absorción por Componente Gigante' (GCA)**. Comparamos rigurosamente nuestra heurística (GCA) contra dos métodos estándar de predicción de enlaces: **Preferential Attachment (PA)** y **Common Neighbors (CN)**.

Los resultados demuestran que, tras un daño severo que fragmenta la red en **994 componentes**, ORT-THERAPY-F **restaura completamente la conectividad global** (reduciendo 993 componentes). En marcado contraste, las estrategias de referencia (PA y CN) **fracasan por completo (0 componentes reducidos)**, demostrando ser ineficaces para esta tarea de reconexión. Además, ORT-THERAPY-F logra esta restauración utilizando un presupuesto de conexión óptimo (**36.5% menos conexiones** que las líneas base) y siendo computacionalmente más rápido.

## 🎯 Contribuciones Principales
* 🧠 **Modelo de Daño Realista:** Simula la neurodegeneración (Alzheimer) como un **Ataque Dirigido a Hubs** (vulnerabilidad de enlaces de alta conectividad), en lugar de un fallo aleatorio.
* 💯 **Fiabilidad Determinista:** Nuestro método (GCA) alcanzó una tasa de éxito de reconexión del **100%** (993 de 993 fragmentos reparados). Las líneas base estándar (PA y CN) **fallaron por completo (0% de éxito)**.
* 💡 **Optimalidad de Recursos:** Logramos una reparación perfecta utilizando un **36.5% menos de conexiones** que las estrategias de referencia, a las cuales se les otorgó un presupuesto mayor y aun así fallaron.
* 🔬 **Distinción del Problema:** Demostramos empíricamente que las estrategias de *densificación* (PA, CN) no son estrategias de *reconexión* (GCA), y fracasan en la tarea de restaurar la integridad estructural global.

## 🔬 Experimento Interactivo y Reproducible
Este repositorio está diseñado para la ciencia abierta y la reproducibilidad total. Puedes ejecutar el pipeline completo del artículo (carga del conectoma, simulación del ataque a hubs y la comparativa de terapias) en el siguiente cuaderno de Google Colab.

**Pipeline de Validación Completo**
Ejecuta el experimento a gran escala para validar cómo ORT-THERAPY-F (GCA) repara el conectoma dañado y por qué fallan las líneas base (PA y CN).
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1v_N-qO_q-Tj1iG2g2e_wY_xKjWq-Z2qB) **<-- (¡RECUERDA ACTUALIZAR ESTE ENLACE AL DE TU NOTEBOOK!)**

## 📂 Estructura del Repositorio
* `ORT_Therapy_Comparison.ipynb`: El cuaderno de Colab interactivo con el experimento central del artículo.
* `bn-human-BNU-1_0025890_session_1.edges`: El dataset del conectoma humano requerido (debe descargarse de [Network Data Repository](https://networkrepository.com/bn-human-BNU-1-0025890-session-1.php)).
* `/data`: Contiene los archivos `.csv` con los resultados detallados generados por el notebook.
* `/figures`: Contiene las figuras generadas para el artículo (como la imagen conceptual de arriba).
* `LICENSE`: La licencia MIT del código.
* `README.md`: Este archivo.

## 🔬 Ciencia Independiente y Abierta
Este trabajo se realizó de manera completamente independiente, sin financiación institucional ni corporativa, demostrando que la investigación de frontera puede surgir también desde entornos abiertos y accesibles. Este proyecto es la aplicación práctica y validación empírica de los principios explorados en el [proyecto Topological Reinforcement Operator](https://github.com/NachoPeinador/Topological-Reinforcement-Operator).

[![Sponsor @NachoPeinador](https://img.shields.io/badge/Sponsor-%E2%9D%A4-%23db61a2.svg)](https://github.com/sponsors/NachoPeinador)

## 🚀 Apoya y Difunde esta Investigación
Como investigador independiente, la visibilidad y el impacto de este trabajo dependen en gran medida del apoyo de la comunidad. Si esta investigación te ha resultado útil o interesante, aquí tienes algunas formas concretas de ayudar:

* **⭐️ Dale una Estrella en GitHub:** Es la forma más rápida y directa de mostrar tu apoyo y ayudar a que otros descubran este proyecto.
* **🔄 Comparte en Redes Sociales:** Publica un enlace al preprint del artículo o a este repositorio en Twitter (X), LinkedIn o tu red académica preferida.
* **✍️ Cita el Trabajo:** Si esta metodología inspira tu propia investigación, la citación es la forma más valiosa de reconocimiento en la ciencia.
* **💬 Inicia una Discusión:** ¿Tienes ideas, preguntas o críticas constructivas? Abre un "Issue" aquí en el repositorio.

**¡Gracias por tu apoyo para hacer visible la ciencia independiente!**

## ✍️ Citación
Si utilizas este trabajo, por favor, cítalo:

**Formato BibTeX**
```bibtex
@article{PeinadorSala2025,
  author    = {Jos\'{e} Ignacio Peinador Sala},
  title     = {Minimal Reconnection for Brain Resilience: A Strategic Reconnection Framework (ORT-THERAPY-F) for Damaged Connectomes},
  journal   = {Zenodo},
  year      = {2025},
  doi       = {10.5281/zenodo.17417142},
  note      = {Repositorio de código y datos: \url{[https://github.com/NachoPeinador/Minimal-Reconnection-for-Brain-Resilience](https://github.com/NachoPeinador/Minimal-Reconnection-for-Brain-Resilience)}}
}
