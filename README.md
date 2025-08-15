# Desafío 1 — Análisis de 4 Tiendas (Data Science LATAM)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Flacoca1970/Desafios_1/blob/main/AluraStoreLatam_Desafio_1_Entrega_Final_v2.ipynb)
[![View on GitHub](https://img.shields.io/badge/GitHub-View%20Notebook-black?logo=github)](https://github.com/Flacoca1970/Flacoca1970/blob/main/AluraStoreLatam_Desafio_1_Entrega_Final.ipynb)
[![Download .ipynb](https://img.shields.io/badge/Download-.ipynb-blue)](https://raw.githubusercontent.com/Flacoca1970/Flacoca1970/main/AluraStoreLatam_Desafio_1_Entrega_Final.ipynb)

**Objetivo**  
Ayudar al Sr. Juan (dueño de 4 minimarkets) a decidir **qué tienda vender** para invertir en un nuevo negocio, usando evidencia basada en datos.

---

## 🔍 Qué hace este proyecto
El notebook realiza, en el orden solicitado, los siguientes análisis **por tienda** usando los datos oficiales publicados en GitHub (no se requiere subir archivos locales):

1. **Análisis de facturación** (total, #ventas, ticket promedio).  
2. **Ventas por categoría** (Top 5 por frecuencia y facturación).  
3. **Calificación promedio de la tienda** (escala 1–5).  
4. **Productos más y menos vendidos** (Top/Bottom 5).  
5. **Costo promedio de envío**.

> Además se incluye un **score opcional** (extensión) para priorizar la decisión de venta combinando: menor facturación, menor calificación y mayor costo de envío.

---

## 🗂️ Datos
Se consumen directamente desde el repositorio oficial (Alura LATAM):

- `tienda_1.csv`  
- `tienda_2.csv`  
- `tienda_3.csv`  
- `tienda_4.csv`

> El notebook carga desde **URLs**; por lo tanto, solo necesitas conexión a internet para reproducir.

---

## 🚀 Cómo ejecutar (recomendado: Google Colab)
1. Abre el notebook en Google Colab.  
2. Ejecuta la celda de **Importación de datos** (carga por URL).  
3. Ejecuta las secciones **1 a 5** en orden.  
4. (Opcional) Ejecuta la sección de **visualizaciones** y el **score** para la recomendación inicial.  
5. Los exportables (CSV/PNG) se guardan en la carpeta `outputs/` (si está habilitado en el notebook).

> Si vas a usar GitHub, agrega un botón “Open in Colab”:  
> `https://colab.research.google.com/github/Flacoca1970/Desafios_1/blob/main/AluraStoreLatam_Desafio_3.ipynb`

---

## 🧠 Metodología (resumen)

**Preparación:** limpieza ligera y tipificación de columnas relevantes (precio, envío, calificación), más detección robusta de nombres con acentos/espacios.  

**Métricas clave:**
- **Facturación Total** (`sum(Precio)`), **#Ventas** y **Ticket Promedio**.
- **Top 5 Categorías** por frecuencia y por facturación.
- **Calificación Promedio** (satisfacción).
- **Costo Promedio de Envío** (eficiencia logística).
- (**Extensión**) **Score “candidata a vender”**: combina *baja facturación*, *baja calificación* y *alto costo de envío* con pesos configurables.

**Visualizaciones:** barras (vertical/horizontal) con etiquetas legibles (miles y CLP), y gráficos Top/Bottom por tienda.

---

## 🏁 ¿Cómo interpretar los resultados?
- **Facturación/Ticket**: bajo desempeño comercial → candidata a vender.  
- **Calificación**: satisfacción baja de clientes → riesgo de retención.  
- **Costo de envío**: alto → ineficiencia logística.  
- **Score combinado (opcional)**: ranking final de candidatas, ponderando las tres dimensiones anteriores.

> **Recomendación**: reportar la tienda con **score más alto** como primera candidata a vender y validar con variables cualitativas (contrato de arriendo, ubicación, proyecciones, personal, etc.).

---

## 📦 Estructura sugerida del repositorio
```
.
├── AluraStoreLatam_Desafio_1.ipynb        # Notebook principal
├── outputs/                                # CSV y PNG generados (opcional)
├── requirements.txt                        # Dependencias mínimas
└── README.md
```

Archivo `requirements.txt` sugerido:
```
pandas
matplotlib
scikit-learn
```

---

## ✅ Buenas prácticas aplicadas
- Carga de datos por **URL oficial** (reproducible).  
- **Detección de columnas** robusta (acentos/espacios).  
- Gráficos con **etiquetas legibles** y formateo CLP/miles.  
- Exportables a `outputs/` para evidencias de evaluación.  

---

## ⚠️ Limitaciones y próximos pasos
- Los datos reflejan el histórico **observado**; no incluyen estacionalidad ni proyecciones.  
- No se modela la **rentabilidad** (margen), solo ventas y costos de envío promedio.  
- Próximos pasos sugeridos:
  - Incorporar **margen por categoría** y **costos fijos** por tienda.
  - Análisis temporal: tendencia y estacionalidad (series de tiempo).
  - Segmentación de clientes/productos (Pareto 80/20, RFM).
  - Sensibilidad del **score** a distintos pesos.

---

## 🧾 Licencia y créditos
Datos provistos por **Alura LATAM — Challenge 1**. Este proyecto se realiza con fines educativos.

---

**Autor:** David González  

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/https://colab.research.google.com/github/Flacoca1970/Flacoca1970/blob/main/AluraStoreLatam_Desafio_1_Entrega_Fina3.ipynb)

> Reemplaza `Flacoca1970/Desafios_1` por tu repositorio real.

**Autor:** David González


[Ver en GitHub](https://github.com/Flacoca1970/Desafios_1/blob/main/AluraStoreLatam_Desafio_1_Entrega_Final_v2.ipynb)
