# 🧴 A/B Testing — La Redoma Rosa 🫧🧴✨

Píldora formativa de **A/B Testing** desarrollada en el Bootcamp de [Factoría F5](https://factoriaf5.org/) de Data Analyst.

Imaginamos **La Redoma Rosa** como una tienda online asturiana de productos  elaborados con ingredientes naturales y recetas tradicionales. El equipo de diseño propone cambiar la estética de la web y, antes de lanzarlo al 100% de los usuarios, realizamos un **A/B test** para decidir con datos, no con opiniones.

---

## 🧪 El experimento

| Versión | Estética | Descripción |
|---------|----------|-------------|
| **A** | Vintage Rosa | Acogedora, retro, evoca naturalidad y tradición |
| **B** | Moderna | Limpia, tecnológica, fría |

**Hipótesis:** La estética vintage (A) generará más conversiones porque transmite los valores de la marca — naturalidad, autenticidad y confianza en los métodos tradicionales.

**Métrica principal:** Tasa de conversión — porcentaje de visitantes que realizan una compra.

---

## 📁 Estructura del repositorio

```
AB_Testing/
│
├── 01_dataset/
│   ├── script_la_redoma_rosa_csv.ipynb   # Generador del dataset sintético
│   └── la_redoma_rosa.csv                # Dataset generado (8.000 registros)
│
├── 02_practica_guiada/
│   └── AB_Testing_La_Redoma_Rosa.ipynb   # Notebook de análisis paso a paso
│
├── imagenes/
│   └── opciones_A_B.png                  # Imagen comparativa de las dos versiones
│
├── presentacion_ab_testing.pdf           # Presentación completa de la píldora formativa
├── .gitignore
└── README.md
```

---

## 🗂️ Dataset

El dataset es **sintético**, generado con Python para simular el comportamiento real de usuarios asturianos. Contiene **8.000 registros** — 4.000 por versión.

| Columna | Descripción |
|---------|-------------|
| `usuario_id` | Identificador único de cada visitante |
| `version` | Versión vista: A (vintage rosa) o B (moderna) |
| `pagina` | Nombre de la versión: `vintage_rosa` o `moderna` |
| `concejo` | Concejo asturiano del visitante |
| `producto_visto` | Producto que estaba mirando |
| `tiempo_sesion_seg` | Segundos que estuvo en la web |
| `convirtio` | 1 si realizó una compra, 0 si no — jerga estándar de marketing digital |

---

## 📓 Práctica guiada

El notebook de análisis sigue cinco pasos:

1. **Cargar y explorar el dataset**
2. **Calcular las métricas por versión**
3. **Visualizar los resultados**
4. **Test estadístico** — z-test de proporciones
5. **Conclusión y decisión final**

### Requisitos

```
pip install -r requirements.txt
```

### Cómo ejecutarlo

1. Ejecuta primero `01_dataset/script_la_redoma_rosa_csv.ipynb` para generar el CSV
2. Abre `02_practica_guiada/AB_Testing_La_Redoma_Rosa.ipynb` y ejecuta las celdas en orden


---

## 🪞 Presentación

La píldora formativa completa está disponible en este repositorio en formato PDF.

Incluye:
- Qué es el A/B Testing y para qué sirve
- Conceptos clave y glosario
- El proceso paso a paso
- Errores frecuentes
- Relación con el análisis de datos

---

## 🌱 Tecnologías

![Python](https://img.shields.io/badge/Python-3.12-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![pandas](https://img.shields.io/badge/pandas-2.x-150458)
![statsmodels](https://img.shields.io/badge/statsmodels-0.14-green)
