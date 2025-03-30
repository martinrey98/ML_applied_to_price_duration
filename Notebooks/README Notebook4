# <ins>**Notebook 4**</ins>: **Modelización** *tradicional de Machine Learning*

### <ins>**Propósito**</ins>

Este notebook tiene como objetivo **desarrollar los modelos tradicionales de Machine Learning** establecidos como objetivo:  
**Extra Trees**, **Decision Tree**, **Random Forest**, **XGBoost**, **LightGBM** y **CatBoost**.  
Se efectúan modelizaciones tanto a nivel **General** (considerando la totalidad de la base) como por **Rubro**.

---

### <ins>**Objetivos**</ins>

- **Modelizar la base** `df_Price_spells_ML.feather` utilizando algoritmos tradicionales de Machine Learning, tanto de forma General como discriminando por *Rubro*.

- **Establecer, para cada modelo**, tanto general como por *Rubro*, **cuál presenta mejor desempeño** entre:  
  **Extra Trees**, **Decision Tree**, **Random Forest**, **XGBoost**, **LightGBM**, **CatBoost**.  
  Para ello se calcula el **MAE** *(Mean Absolute Error)* con el objetivo de determinar cuál de los modelos alcanza un menor valor en dicho indicador.

- **Calcular la relevancia de los predictores** para los modelos ganadores, tanto en el modelo general como por rubro.

---

### <ins>**Archivos necesarios**</ins>

1. `df_Price_spells_ML.feather` → Base con las series temporales de Price Spells depurada (sin outliers ni censura), generada en el `Notebook 2`.

---

### <ins>**Archivos generados**</ins>

#### 1. **Archivos `.pkl` con los modelos entrenados (General y por Rubro)**

**Modelos generales:**
- `Decision_Tree_model_base.pkl`
- `Extra_Trees_model_base.pkl`
- `Random_Forest_model_base.pkl`
- `XGBoost_model_base.pkl`
- `LightGBM_model_base.pkl`
- `CatBoost_model_base.pkl`
- `Decision_Tree_best_model.pkl`
- `Extra_Trees_best_model.pkl`
- `Random_Forest_best_model.pkl`
- `XGBoost_best_model.pkl`
- `LightGBM_best_model.pkl`
- `CatBoost_best_model.pkl`

**Modelos por *Rubro*:** (para *alimentos, bebidas_con_alcohol, bebidas_sin_alcohol, cuidado_personal, limpieza*)
- `Decision_Tree_best_model_<rubro>.pkl`
- `Extra_Trees_best_model_<rubro>.pkl`
- `Random_Forest_best_model_<rubro>.pkl`
- `XGBoost_best_model_<rubro>.pkl`
- `LightGBM_best_model_<rubro>.pkl`
- `CatBoost_best_model_<rubro>.pkl`

---

#### 2. **Importancia de los predictores (gráficos)**

- `Importancia_Predictores.png` → General  
- `Importancia_Predictores_<rubro>.png` → Por rubro

---

#### 3. **Resumen de Resultados (Excel)**

- `Resumen_Resultados.xlsx` → Consolidado con métricas por modelo y rubro:  
  *MAE, R², RMSE, MAPE*, características de cada modelo.

---

#### 4. **Comparación Train vs Test (Solo modelo general)**

- `Comparative Results (Train vs Test).xlsx` → Comparativa entre desempeño en entrenamiento y prueba.

---
