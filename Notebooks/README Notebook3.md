# <ins>**Notebook 3**</ins>: **Análisis estadístico de base** ***Price Spells***

### **<ins>Propósito</ins>**

Este notebook tiene como objetivo **<ins>analizar las principales características de las variables empleadas en las modelizaciones de Machine Learning desarrolladas.</ins>** Como fue definido en la sección de  `Transformación y limpieza de los datos`, la base de *Price Spells* utilizada está compuesta por intervalos de precios para cada combinación existente de establecimiento-producto, siendo la variación de dichos precios lo que da inicio y fin a cada uno de los intervalos.

**<ins>El análisis exploratorio fue realizado sobre la base de datos utilizada para la modelización tradicional de Machine Learning</ins>**, la cual consiste en todas las combinaciones establecimiento-producto clasificadas como *Completed*, posterior a la depuración realizada por concepto de  *Outliers* y datos censurados.

**<ins>Las variables predictoras utilizadas para la modelización son:</ins>** *Categoría, Promoción, Cadena, Tipo de Establecimiento, Municipio, Mes, Día del Mes, Día de Semana, Var Precio % y Lag Duración1*.

---

### **<ins>Objetivos</ins>**

- **<ins>Analizar el comportamiento de las variables empleadas en el desarrollo de modelos tradicionales de Machine Learning.</ins>** **En especial su vinculación con la variable a predecir *Duración***.
- **<ins>Perfilar las variables que pueden llegar a instrumentarse en las modelizaciones de Machine Learning</ins>**, teniendo en consideración la relación entre estas y *Duración*.
- **<ins>Generar tablas y figuras resumen que se incorporaron en la tésis.</ins>**

---

### **<ins>Archivos necesarios</ins>**

1. **<ins>establecimiento.xlsx</ins>** -> Listado de establecimientos en base
2. **<ins>productos.csv</ins>** -> Listado de productos en base
3. **<ins>productos (Rubros y Categorías).csv<ins>** -> Contiene los Rubros y
Categorias asociados a cada uno de los productos en base
4. **<ins>Feriados.csv<ins>** -> Listado con los días feriados del período analizado
5. **<ins>Grilla de Productos.csv<ins>** -> Listado de productos considerados en el estudio
7. **<ins>df_Price_spells_SML.feather</ins>** -> Base que contiene las series temporales de Price Spells de los pares establecimiento-producto en Montevideo, correspondientes al período enero 2021 - junio 2024. Se utiliza para la modelización Survival Machine Learning.
2. **<ins>df_Price_spells_ML.feather</ins>** -> Base que contiene las series temporales de Price Spells de los pares establecimiento-producto en Montevideo, correspondientes al período enero 2021 - junio 2024. Se utiliza para la modelización tradicional de Machine Learning.

---

### **<ins>Archivos generados</ins>**

**<ins>Gráficas y tablas de:</ins>**

(generados en el entorno de trabajo)

- Estadísticos generales de la variable *Duración* y discriminados por la   variable *Promoción*
- Distribución de la base por *Rubro*; por *Día de la Semana*; por *Incremento* y *Reducción* de *Precio*; por *Cadena*; por *Tipo de Establecimiento*; por *Municipio*.
- Distribución de la *Duración* de los spells (Histograma)
- Evolución general y por rubros de la *Duración* promedio de los spells (Gráfico de líneas)
- Distribución de las duraciones de los spells por *Categoría* (Boxplot)
- Cantidad de spells por *Día del Mes* (Barras)
- Cantidad de spells y *Duración* media por *Mes* (Barras)
- Distribución de spells por *Categoría* (Barras)
- Mapas de calor por Rubros con la relación entre *Duración*, *Categoría* y *Tipo de Establecimiento*
- Relación entre la media de la *Duración* y la media de *Var_Precio_%* por Rubros discriminando entre Incrementos y Reducciones (Puntos)


---
