# 📡 Telecom X Parte 2: Inteligencia Predictiva aplicada a la Retención de Clientes (Churn)

**Consultor de Datos:** Mateo Pulgarin Garcia
**Proyecto:** Desafío Telecom X – Fase de Modelado y Estrategia Comercial

---

## 🧠 Contexto y Visión General

Este proyecto representa la etapa avanzada del desafío **Telecom X**, centrada en la construcción de un ecosistema de **Machine Learning** para mitigar la deserción de clientes. El objetivo central es transformar datos históricos en inteligencia predictiva, permitiendo que la organización anticipe el *churn* y ejecute acciones de retención personalizadas y proactivas.

El flujo de trabajo abarca desde la ingeniería de atributos y el tratamiento del desbalance de clases, hasta la validación cruzada de modelos bajo métricas de negocio rigurosas.

---

## 🎯 Objetivos Estratégicos

* **Pipeline de Datos:** Preparación, limpieza y codificación de variables para algoritmos de clasificación.
* **Análisis de Desbalance:** Tratamiento del impacto estadístico de las clases minoritarias para evitar sesgos.
* **Benchmarking de Modelos:** Comparativa técnica entre modelos Baseline, Árboles de Decisión y Regresión Logística.
* **Optimización de Métricas:** Foco prioritario en **Recall** y **F1-Score** para garantizar la detección efectiva de cancelaciones.
* **Insights de Negocio:** Identificación de las variables con mayor peso estadístico en la decisión de salida del cliente.

---

## 🛠️ Metodología y Modelado

Para garantizar la robustez de las predicciones, el proyecto siguió una arquitectura de análisis detallada:

### 1. Selección de Algoritmos
Se evaluaron diferentes enfoques para encontrar el equilibrio ideal entre precisión y capacidad de detección:
- **Modelo Baseline:** Utilizado como punto de referencia y diagnóstico del desbalance de clases.
- **Árbol de Decisión:** Implementado para capturar relaciones no lineales y ofrecer una estructura clara de decisión.
- **Regresión Logística (Seleccionado):** Consolidado como la solución óptima debido a su balance superior entre métricas y estabilidad operativa.

### 2. Análisis de Performance
La evaluación se profundizó mediante **matrices de confusión (absolutas y normalizadas)**. Este enfoque permitió auditar la tasa de acierto en clientes que realmente pretenden cancelar, eliminando los ruidos visuales producidos por el tamaño de la cartera de clientes activos.

---

## 📈 Hallazgos e Inteligencia de Datos

El modelo permitió aislar los patrones críticos que definen el perfil de riesgo en Telecom X:
* **Factor Temporal:** Los clientes con **baja antigüedad** presentan la mayor vulnerabilidad, especialmente durante los primeros meses de relación.
* **Estructura Contractual:** Los contratos mensuales (corto plazo) se identifican como los principales vectores de evasión.
* **Sensibilidad Financira:** Existe una correlación directa entre cargos mensuales elevados y una mayor propensión al abandono.
* **Barrera de Retencción:** La permanencia prolongada y los contratos de larga duración actúan como protectores naturales de la lealtad.

---

## 💡 Recomendaciones Estratégicas

A partir de los hallazgos, se sugieren las siguientes acciones para **Telecom X**:

1.  **Blindaje de Clientes Nuevos:** Implementar protocolos de *onboarding* y beneficios exclusivos durante el primer trimestre de contrato.
2.  **Conversión Contractual:** Incentivar la migración de planes mensuales a esquemas anuales mediante incentivos económicos o mejoras de servicio.
3.  **Sistema de Alerta Temprana (EWS):** Integrar el modelo de Regresión Logística al CRM para priorizar la atención de clientes identificados como de "Alto Riesgo".
4.  **Optimización del Valor Percibido:** Promover la contratación de servicios combinados (*bundling*) para aumentar la vinculación y el valor de vida del cliente (LTV).

---

## 💻 Stack Tecnológico

* **Lenguaje:** Python
* **Manipulación de Datos:** Pandas, NumPy
* **Machine Learning:** Scikit-learn
* **Visualización:** Matplotlib, Seaborn
* **Entorno:** Google Colab
