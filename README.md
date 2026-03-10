Telecom X – Predicción de Cancelación de Clientes (Churn)
📌 Descripción del Proyecto

Este proyecto tiene como objetivo predecir qué clientes de Telecom X tienen mayor probabilidad de cancelar sus servicios. Utilizando datos históricos de clientes, se construyeron modelos de machine learning para anticipar la cancelación y ayudar a la empresa a diseñar estrategias de retención efectivas.

El análisis se realiza en dos etapas:

Análisis Exploratorio de Datos (EDA): Comprender la distribución de los clientes, detectar patrones y evaluar factores que afectan la cancelación.

Modelado Predictivo: Entrenar y evaluar modelos de clasificación para predecir la probabilidad de churn, incluyendo interpretación de variables relevantes.

🧰 Tecnologías y Librerías

Python 3.x

Librerías principales:

pandas y numpy → manejo y limpieza de datos

matplotlib y seaborn → visualización de datos

scikit-learn → preprocesamiento, modelado y evaluación

imbalanced-learn → manejo de desbalanceo de clases (opcional)

⚙️ Preparación de Datos

Se cargó el dataset TelecomX_Clean.csv con información de clientes.

Se eliminaron columnas irrelevantes como customerID.

Variables categóricas se convirtieron en dummies (One-Hot Encoding) para compatibilidad con modelos.

Se normalizaron variables numéricas (tenure, Charges.Monthly, Charges.Total) para modelos sensibles a escala.

Se verificó balance de clases en Churn y se aplicaron técnicas de balanceo cuando fue necesario.

📊 Análisis Exploratorio

Se realizaron visualizaciones para entender:

Distribución de clientes que cancelaron vs los que permanecieron.

Relación de churn con variables categóricas: género, tipo de contrato, método de pago, servicios adicionales.

Relación de churn con variables numéricas: tiempo de contrato, gasto mensual y total.

🧠 Modelos Entrenados

Se evaluaron dos modelos principales:

Regresión Logística

Métricas de desempeño:

Accuracy: 80%

ROC-AUC: 0.845

Variables más influyentes: InternetService_Fiber optic, Charges.Total, PaperlessBilling.

Random Forest

Métricas de desempeño:

Accuracy: 79%

ROC-AUC: 0.823

Variables más importantes: InternetService_Fiber optic, Charges.Total, PaperlessBilling.

Se observó que clientes con internet de fibra óptica, facturación sin papel y altos gastos totales presentan mayor riesgo de cancelación.

💡 Conclusiones

Los principales factores que influyen en la cancelación son:

Tipo de servicio de internet (Fibra óptica aumenta riesgo)

Gasto total del cliente

Facturación electrónica (PaperlessBilling)

Método de pago (Electronic check)

Las estrategias de retención deben enfocarse en estos segmentos de clientes para reducir la evasión.

📝 Recomendaciones

Ofrecer beneficios o descuentos a clientes con contratos de alto gasto o fibra óptica.

Incentivar formas de pago más seguras o automatizadas para clientes con pagos electrónicos.

Monitorear clientes con PaperlessBilling y ofrecer atención personalizada para evitar cancelaciones.
