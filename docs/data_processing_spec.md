# Especificación de Procesamiento de Datos

## Objetivo

Este documento resume las reglas de preparación de datos que sustentan la base analítica del proyecto. Su propósito es alinear el notebook, el dataset procesado y la futura sincronización con Power BI bajo una misma lógica de negocio.

## Arquitectura del flujo

El flujo analítico del proyecto sigue una estructura simple y reproducible:

1. `data/raw/marketing_raw.csv` se conserva como fuente original e inmutable.
2. `notebooks/01_eda_preprocessing.ipynb` ejecuta la auditoría, limpieza, reconstrucción de variables y validaciones.
3. `data/processed/marketing_clean.csv` se genera como salida analítica oficial para consumo en Power BI y en la documentación del proyecto.

## Política de duplicados

- El archivo raw no se modifica.
- La versión analítica elimina únicamente duplicados exactos.
- El dataset procesado esperado contiene `2021` filas después de la deduplicación exacta.
- No se debe afirmar que el dataset original está libre de duplicados sin distinguir entre la fuente raw y la salida procesada.

## Transformaciones aplicadas

- Conversión de variables monetarias de texto a formato numérico:
  - `Income`
  - `MntWines`
  - `MntFruits`
  - `MntMeatProducts`
  - `MntFishProducts`
  - `MntSweetProducts`
  - `MntGoldProds`
  - `MntTotal`
- Reconstrucción de `Marital_Status` a partir de `marital_*`.
- Reconstrucción de `Education_Level` a partir de `education_*`, incluyendo `education_2n Cycle`.
- Eliminación de columnas one-hot maritales y educativas en la salida analítica final para evitar redundancia y ambigüedad.

## Variables derivadas

- `Has_Children`: identifica hogares con al menos un niño o adolescente.
- `Age_Group`: segmentación etaria para comparar comportamiento de compra por rangos.
- `Customer_Tenure_Years`: antigüedad del cliente expresada en años.
- `Customer_Tenure_Group`: clasificación relativa respecto a la mediana de `Customer_Days`.
- `Is_High_Value_Customer`: identifica clientes cuyo `MntTotal` está en o por encima del percentil 75.
- `Premium_Spend_Share`: proporción del gasto premium (`MntGoldProds`) sobre el gasto total.

## Reglas de validación

- Cada fila debe tener exactamente una categoría marital activa.
- Cada fila debe tener exactamente una categoría educativa activa.
- No se deben introducir nulos nuevos durante la limpieza.
- El valor `Age = 99999` no aparece en el raw actual; por tanto, no se considera un problema activo en esta versión.
- El dataset final debe poder exportarse y leerse nuevamente sin pérdida de columnas ni inconsistencias de forma.

## Definiciones analíticas clave

- `Average Income`: promedio de `Income` en el dataset procesado.
- `Average Total Spend`: promedio de `MntTotal`.
- `High-Value Customer Rate`: proporción de clientes marcados como `Is_High_Value_Customer`.
- `Premium Spend Share`: promedio de `Premium_Spend_Share`.
- `Customers With Children`: proporción de clientes donde `Has_Children = True`.
- `Web vs Store Mix by Age Group`: participación relativa de `NumWebPurchases` y `NumStorePurchases` dentro de cada `Age_Group`.
- `Average Discount Purchases by Segment`: promedio de `NumDealsPurchases` por segmento analítico.

## Utilidad dentro del repositorio

Este documento cumple dos funciones:

- explicar la limpieza de datos realizada desde el notebook
- servir como referencia técnica para alinear el dashboard, el README y la narrativa del portafolio
