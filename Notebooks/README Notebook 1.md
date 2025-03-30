# <ins>**Notebook 1**</ins>: **Consolidación de Base de Precios**

### **<ins>Propósito</ins>**

Este notebook tiene como objetivo **consolidar las bases de datos originalmente elaboradas por el** **SIPC** *(Sistema de Información de Precios al Consumidor)* **de forma anual**, a fin de **generar una única base de precios para la totalidad del período en estudio:** ***Enero 2021 - Junio 2024***, imponiéndose diversos criterios de selectividad y completando faltantes en caso de haberlos.

---

### **<ins>Objetivos</ins>**

- **Consolidar en un solo dataframe la totalidad de bases de datos** referentes al período estudiado: *Enero 2021 - Junio 2024*  
- **Establecer y ejecutar un proceso de depuración** sobre los datos obtenidos, con el objetivo de consolidar una base de datos con la calidad suficiente que permita, a posteriori, la conformación de bases de *Price Spells*, las cuales serán utilizadas para la modelización en Machine Learning y Survival Machine Learning  
- **Efectuar un pequeño análisis estadístico** sobre las bases formuladas a fin de conocer sus características y diferencias principales.

---

### **<ins>Archivos necesarios</ins>**

1. `establecimiento.xlsx` → Listado de establecimientos en base  
2. `productos.csv` → Listado de productos en base  
3. `productos (Rubros y Categorías).csv` → Contiene los Rubros y Categorías asociados a cada uno de los productos en base  
4. `precios_2021.csv` → Precios reportados por el SIPC para 2021  
5. `precios_2022.csv` → Precios reportados por el SIPC para 2022  
6. `precios_2023.csv` → Precios reportados por el SIPC para 2023  
7. `precios_2024.csv` → Precios reportados por el SIPC para el primer semestre de 2024  

---

### **<ins>Archivos generados</ins>**

1. `df_precios_montevideo_2021_2024_C.feather` → Base con la totalidad de precios sin agrupar de los pares establecimiento-producto en Montevideo para el período Enero 2021 - Junio 2024, que cumplen con las restricciones establecidas en el presente Notebook.
