# 🌿 Análisis Exploratorio de Calidad del Aire - Phoenix, AZ

Este proyecto analiza datos de calidad del aire en Phoenix (Arizona, EE.UU.), usando Python y `ydata-profiling`.

---

## 📁 Archivos incluidos

- `EDA_Contaminacion_USA.html`: Informe EDA automático  
- `PythonProjectN1.ipynb`: Código de limpieza, análisis y visualización  
- `Documentacion.pdf`: Documentación del proyecto  
- `El dataset se encuentra en una carpeta de Drive, ya que sobrepasa los 100MB, se descarga ya en el notebook`: Dataset (1000 registros)

---

## 🔧 Limpieza aplicada

- Eliminadas columnas constantes: `State`, `City`, `Address`
- Filas con nulos en `SO2 AQI` y `CO AQI` fueron removidas
- `Date Local` convertida a tipo `datetime`

---

## 📊 Principales hallazgos

- Alta correlación entre `CO AQI`, `CO Mean` y `CO 1st Max Value`
- Frecuencia alta de ceros en varias columnas (ej. `SO2 AQI`, `CO 1st Max Hour`)
- Visualizaciones muestran distribuciones sesgadas a valores bajos

---

## ✅ Conclusiones

- El aire en Phoenix muestra generalmente bajos niveles de contaminación
- Hay redundancia útil entre variables que puede aprovecharse en modelos
- Se recomienda extender el análisis a otras ciudades

---

## 🛠 Requisitos

```bash
pip install pandas seaborn ydata-profiling matplotlib
