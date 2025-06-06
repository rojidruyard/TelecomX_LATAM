
# 📊 Análisis de Evasión de Clientes - TelecomX

Este proyecto analiza los datos de clientes de **TelecomX**, una empresa ficticia de telecomunicaciones, con el objetivo de identificar **patrones de cancelación de servicio (Churn)** y generar **recomendaciones estratégicas** basadas en datos.

---

## 🧠 Objetivo

- Estudiar los factores que influyen en la evasión de clientes.
- Explorar variables categóricas y numéricas que afectan el churn.
- Visualizar patrones de comportamiento en la base de clientes.
- Proponer estrategias para **reducir la tasa de cancelación**.

---

## 📁 Estructura del proyecto

- `TelecomX_Data.json`: archivo original con los datos en formato JSON anidado.
- `notebook_analisis.ipynb`: contiene todo el análisis paso a paso.
- `README.md`: este archivo.

---

## ⚙️ Tecnologías usadas

- Python
- pandas
- plotly (para visualizaciones interactivas)
- Jupyter Notebook

---

## 🧼 Limpieza y preparación de datos

- Normalización de estructuras JSON anidadas con `pd.json_normalize`.
- Conversión de datos numéricos (`Charges.Total`, `MonthlyCharges`) a `float`.
- Cálculo de nueva variable `Cuentas_Diarias` para analizar el gasto diario estimado.
- Eliminación de inconsistencias y control de valores nulos.

---

## 📊 Análisis Exploratorio

### Variables categóricas analizadas:

- Género (`gender`)
- Tipo de contrato (`Contract`)
- Método de pago (`PaymentMethod`)
- Uso de facturación electrónica (`PaperlessBilling`)

### Variables numéricas analizadas:

- Tiempo de contrato (`tenure`)
- Cargos mensuales (`MonthlyCharges`)
- Total gastado (`Charges.Total`)
- Gasto diario (`Cuentas_Diarias`)

Se generaron **gráficos interactivos** para comparar estas variables según el estado de churn (Sí/No).

---

## 💡 Conclusiones

- Clientes con **poca antigüedad** y contratos **mes a mes** presentan mayor riesgo de evasión.
- El método de pago **Electronic check** se asocia a alta cancelación.
- **Altos cargos mensuales** con **bajo gasto acumulado** reflejan una posible insatisfacción temprana.

---

## ✅ Recomendaciones

- Aplicar estrategias de retención a clientes nuevos (bonificaciones, soporte personalizado).
- Incentivar métodos de pago automáticos y contratos anuales.
- Crear alertas internas para clientes con alto riesgo (basado en perfiles detectados).

---

## 🚀 Próximos pasos

- Entrenamiento de un **modelo predictivo de churn** con machine learning.
- Implementación de un dashboard interactivo con Plotly Dash o Power BI.
- Automatización de alertas para el equipo de atención al cliente.

---

## ✍️ Autor

**[Tu Nombre Aquí]**  
Análisis realizado como parte del desafío de ciencia de datos para TelecomX.  
