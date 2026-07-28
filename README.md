# ⚡ El Expediente Tucumán 2027: Sistema de Soporte a las Decisiones

![UTN FRT](https://img.shields.io/badge/UTN-FRT-blue?style=for-the-badge)
![Investigación Operativa](https://img.shields.io/badge/Investigación_Operativa-4K1-004e89?style=for-the-badge)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

Landing Page interactiva y repositorio del **Trabajo Final Integrador** para la cátedra de Investigación Operativa (Ingeniería en Sistemas de Información - Universidad Tecnológica Nacional, Facultad Regional Tucumán).

🔗 **[Ver la Landing Page en Vivo (GitHub Pages)](https://[TU-USUARIO].github.io/tfi-invop/)**

## 📋 Sobre el Proyecto

La provincia de Tucumán presenta una problemática estructural en su sistema de distribución eléctrica, caracterizada por picos críticos de demanda en la temporada estival que saturan la red de transporte. A esto se suma el desafío regulatorio de la **Ley N.º 27.191**, que exige el despacho preferencial de energías renovables locales (Hidráulica, Biomasa y Biogás).

Este proyecto reemplaza la toma de decisiones empírica por un **Sistema de Soporte a las Decisiones (SSD)** basado en modelos matemáticos, diseñado para minimizar los costos operativos y gestionar el riesgo de desabastecimiento.

## 🚀 Módulos del Sistema

El SSD está compuesto por tres modelos secuenciales y un simulador interactivo:

1. **Módulo Predictivo (Pronóstico Climático):** Modelo temporal de regresión con variable exógena estival. Proyecta la demanda mensual de 2027 con un MAPE validado del 3%.
2. **Gestión de Riesgo (Modelo Newsvendor):** Modelo estocástico que determina el nivel óptimo de reserva térmica mensual (entre 42 y 51 GWh) balanceando el Costo de Energía No Suministrada (CENS) frente al costo de capacidad ociosa.
3. **Optimización (Programación Lineal Multiperíodo):** Modelo resuelto vía Solver que minimiza el costo total de adquisición, demostrando que cumplir con la cuota de renovables implica un sobrecosto operativo del **+3,63%** anual, pero fomenta la descarbonización local.
4. **Análisis de Sensibilidad (Dashboard):** Simulador web que somete al sistema a estrés (picos de calor + fallas de transporte), revelando que **la vulnerabilidad estructural reside en la red de transporte**, multiplicando el déficit energético de forma no lineal (5.3x) ante contingencias combinadas.

## 🛠️ Tecnologías Utilizadas

*   **Modelado y Resolución:** Microsoft Excel (Solver, Análisis de Datos).
*   **Frontend (Landing Page):** HTML5, CSS3 (Vanilla, UI/UX tipo Dashboard SaaS).
*   **Interactividad:** JavaScript ES6.
*   **Visualización de Datos:** [Chart.js](https://www.chartjs.org/).
*   **Renderizado Matemático:** [KaTeX](https://katex.org/).

## 📁 Estructura del Repositorio

```text
📦 tfi-invop
 ┣ 📜 index.html                                  # Código fuente de la Landing Page interactiva
 ┣ 📜 TFI-Bustos-Cedron-Fenino-Gallardo... .xlsx  # Libro de cálculo con los modelos matemáticos y Solver
 ┣ 📜 AV3-Bustos-Cedron-Fenino-Gallardo... .docx  # Documento de investigación formal (Paper)
 ┗ 📜 README.md                                   # Documentación del repositorio
