# <ins>**Notebook 5**</ins>: **Modelización** *Survival Machine Learning*

### <ins>**Propósito**</ins>

Este notebook tiene como objetivo **desarrollar los modelos de Survival Machine Learning** establecidos como objetivo:  
**Random Survival Forest (RSF)** y **Cox Proportional Hazards**.  
Se efectúan modelizaciones tanto a nivel **General** (considerando la totalidad de la base) como por **Rubro**.

---

### <ins>**Objetivos**</ins>

- **Modelizar la base** `df_Price_spells_SML.feather` utilizando algoritmos de Survival Analysis, tanto de forma general como discriminando por *Rubro*.

- **Establecer, para cada modelo**, general o por *Rubro*, cuál presenta mejor desempeño entre:
  - **Random Survival Forest (RSF)**
  - **Cox Proportional Hazards**  
  Para ello se calcula el **C-Index**, buscando el mayor valor posible como indicador de buen desempeño.

- **Determinar el valor del MAE Uncensored** para todos los modelos, utilizando la librería `SurvivalEVAL`, con el objetivo de comparar estos resultados con los obtenidos en el `Notebook 4: Modelización tradicional de Machine Learning`.

---

### <ins>**Archivos necesarios**</ins>

1. `df_Price_spells_SML.feather` → Base con series temporales de Price Spells (sin restricciones), generada en el `Notebook 2`, correspondiente a *Enero 2021 - Junio 2024*.

---

### <ins>**Archivos generados**</ins>

#### 1. **Modelos `.pkl` entrenados (General y por Rubro)**

Para cada *Rubro* analizado (*alimentos, bebidas_con_alcohol, bebidas_sin_alcohol, cuidado_personal, limpieza*) y para el modelo general, se generan:

- `Random_Survival_Forest_<rubro o general>.pkl`  
- `Cox_Proportional_Hazards_Model_<rubro o general>.pkl`

---

#### 2. **Gráficos de curvas de supervivencia**

Generación de gráficos `.png` con las curvas estimadas:

- `Random_Survival_Forest_Curva_de_Supervivencia_<rubro o general>.png`  
- `Cox_Proportional_Hazards_Model_Curva_de_Supervivencia_<rubro o general>.png`

---

#### 3. **Resumen de Resultados (Excel)**

- `Resumen_Resultados.xlsx` → Contiene:  
  *C-Index*, *MAE Uncensored*, características del modelo.

---

#### 4. **Comparativa Train vs Test (General y por Rubro)**

- `Comparative Results (Train vs Test).xlsx` → Comparación de desempeño entre entrenamiento y prueba para todos los modelos.

---
