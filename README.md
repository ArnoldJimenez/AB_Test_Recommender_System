# 🧪 Análisis de Embudo de Conversión y Prueba A/B

![Python](https://img.shields.io/badge/Python-3.9+-blue?logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)
![ABTest](https://img.shields.io/badge/A%2FB-Testing-red)
![Status](https://img.shields.io/badge/Project-Completed-brightgreen)

Este proyecto analiza el **embudo de conversión de un e-commerce** y evalúa mediante una **prueba A/B** el impacto de un nuevo sistema de recomendaciones en el comportamiento de los usuarios.  

---

## 🚀 Conclusiones principales

### 🔍 Exploración de datos (EDA)
- ✅ Usuarios válidos tras limpieza: **~3,481 usuarios y 21,952 eventos** → base depurada y consistente.  
- 📊 Distribución de eventos: predominan **login** y **product_page**, con menos usuarios llegando a **purchase** → se confirma estructura de embudo.  
- 🛒 Embudo global:
  - ~62% visitan la **página de producto**.  
  - ~29% añaden al **carrito**.  
  - ~31% completan la **compra**.  
- ⚖️ Balance de grupos:  
  - El grupo A tiene más usuarios que el grupo B.  
  - Ambos presentan un comportamiento similar en eventos por usuario.  
  - No se detectaron **usuarios duplicados**.  
- ⏳ Distribución temporal: mayor actividad entre **14 y 21 de diciembre**, coincidiendo con pico de inscripciones.  

---

### 📈 Resultados de la prueba A/B
- 🔢 **Tasas de conversión por etapa**:
  - `product_page`: A (64.8%) > B (56.4%).  
  - `product_cart`: A (30.0%) ~ B (27.5%).  
  - `purchase`: A (31.7%) > B (27.6%).  

- 🧮 **Prueba Z**:
  - `product_page`: diferencia **significativa** (p < 0.001).  
  - `product_cart`: diferencia **no significativa** (p = 0.145).  
  - `purchase`: diferencia **significativa** (p = 0.018).  

---

### 🧐 Interpretación
- El **nuevo sistema de recomendaciones (grupo B)** **NO cumple** con la hipótesis de mejorar la conversión en +10%.  
- Por el contrario:  
  - Reduce la conversión en **product_page** y **purchase** de forma significativa.  
  - No genera mejoras en **product_cart**.  
- Conclusión: la implementación del nuevo sistema **no es recomendable en su estado actual**.  

---

## 📂 Contenido del repositorio
- 📁 `notebooks/` → Análisis exploratorio (EDA) y prueba A/B en Jupyter.  
- 📁 `data/` → Dataset anonimizado con usuarios y eventos.  
- 📁 `reports/` → Visualizaciones y reportes finales.  

---

## ✨ Tecnologías utilizadas
- **Python** 🐍 (pandas, numpy, scipy, statsmodels)  
- **Jupyter Notebook** 📓  
- **Matplotlib & Seaborn** 📊  
- **Pruebas estadísticas (Z-test, conversión por etapas)**  

---

## 📌 Autor
**Arnold Joel Jimenez**  
📍 Analista de Datos | Bogotá, Colombia  

