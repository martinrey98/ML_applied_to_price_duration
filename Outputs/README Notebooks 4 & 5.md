# <ins>**Outputs – Notebooks 4 y 5**</ins>

⚠️ **Nota:** Los archivos `.pkl` generados en el presente trabajo **no se encuentran subidos debido a su tamaño**.  
 Para más información, véase: [*README Databases*](./README_Databases.md)

---

## <ins>**Notebook 4**</ins>: *Modelización tradicional de Machine Learning*

### <ins>**1. Modelos entrenados (`.pkl`)**</ins>

#### **Modelos generales:**
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

#### **Modelos por *Rubro*:**  
(*alimentos, bebidas_con_alcohol, bebidas_sin_alcohol, cuidado_personal, limpieza*)

- `Decision_Tree_best_model_<rubro>.pkl`
- `Extra_Trees_best_model_<rubro>.pkl`
- `Random_Forest_best_model_<rubro>.pkl`
- `XGBoost_best_model_<rubro>.pkl`
- `LightGBM_best_model_<rubro>.pkl`
- `CatBoost_best_model_<rubro>.pkl`


### <ins>**2. Importancia de predictores (`.png`)**</ins>
- `Importancia_Predictores.png`
- `Importancia_Predictores_<rubro>.png`


### <ins>**3. Resultados (`.xlsx`)**</ins>
- `Resumen_Resultados.xlsx`  
  → Incluye métricas: *MAE*, *R²*, *RMSE*, *MAPE*, características por modelo y rubro.

- `Comparative Results (Train vs Test).xlsx`  
  → Comparación de desempeño en *Train* vs *Test* (solo modelo general).

---

## <ins>**Notebook 5**</ins>: *Modelización Survival Machine Learning*

### <ins>**1. Modelos entrenados (`.pkl`)**</ins>

#### **Modelos generales y por rubro:**
- `Random_Survival_Forest_<rubro o general>.pkl`
- `Cox_Proportional_Hazards_Model_<rubro o general>.pkl`

### <ins>**2. Curvas de supervivencia (`.png`)**</ins>

- `Random_Survival_Forest_Curva_de_Supervivencia_<rubro o general>.png`
- `Cox_Proportional_Hazards_Model_Curva_de_Supervivencia_<rubro o general>.png`

### <ins>**3. Resultados (`.xlsx`)**</ins>

- `Resumen_Resultados.xlsx`  
  → Incluye métricas: *C-Index*, *MAE Uncensored*, características por modelo y rubro.

- `Comparative Results (Train vs Test).xlsx`  
  → Comparación entre desempeño en entrenamiento (*Train*) y prueba (*Test*).

---
