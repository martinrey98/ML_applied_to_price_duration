# <ins>**Notebook 2**</ins>: **Generación de Bases de Price Spells**

### **<ins>Propósito</ins>**

Este notebook tiene como objetivo **generar las bases de datos de Price Spells a partir de las bases consolidadas de precios diarios generadas en el Notebook 1**, las cuales serán utilizadas para las modelaciones de Machine Learning.  
Para ello, se definen spells o intervalos ante cada cambio de precio, para cada combinación establecimiento-producto.

---

### **<ins>Objetivos</ins>**

- **Generar series temporales de Price Spells** para el período *Enero 2021 - Junio 2024*, incorporando las siguientes variables:
  - *Barrio*
  - *Municipio*
  - *Intervalo*
  - *Fecha_inicio*
  - *Fecha_fin*
  - *Lag_Duración1*         
  - *Rolling_Mean_Duración*
  - *Var_Precio*
  - *Var_Precio_%*
  - *Incremento*
  - *Reducción*
  - *Var_+_10%*
  - *Censurado*
  - *Año*
  - *Trimestre*
  - *Mes*
  - *Día_del_mes*
  - *Día_de_la_semana*
  - *Feriado*

- **Conocer el comportamiento de la variable `Duración`** (variable a predecir), según los distintos valores de la variable dummy `Promoción`, con el objetivo de eliminar valores *outliers* discriminando por los posibles valores de esta última (*No Promoción = 0 | Promoción = 1*).

- **Definir las bases para el desarrollo de modelos:**
  - **Modelos Survival**: base de datos *Price Spells* sin restricciones → `df_Price_spells_SML.feather`
  - **Modelos tradicionales de Machine Learning**: base de datos *Price Spells* depurada (sin outliers ni censura) → `df_Price_spells_ML.feather`

- **Efectuar un pequeño análisis estadístico** sobre las bases formuladas para conocer sus características y diferencias principales.

---

### **<ins>Archivos necesarios</ins>**

1. `establecimiento.xlsx` → Listado de establecimientos en base  
2. `productos.csv` → Listado de productos en base  
3. `productos (Rubros y Categorías).csv` → Rubros y categorías de productos  
4. `Feriados.csv` → Días feriados del período  
5. `Grilla de Productos.csv` → Productos considerados en el estudio  
6. `df_precios_montevideo_2021_2024_C.feather` → Base consolidada de precios por par establecimiento-producto en Montevideo (generada en Notebook 1)

---

### **<ins>Archivos generados</ins>**

1. `df_Price_spells_SML.feather` → Base con series temporales de Price Spells de los pares establecimiento-producto en Montevideo (Ene 2021 – Jun 2024).  
   **Se utiliza para la modelización Survival Machine Learning.**

2. `df_Price_spells_ML.feather` → Base similar a la anterior pero depurada (sin outliers ni spells censurados).  
   **Se utiliza para la modelización tradicional de Machine Learning.**
