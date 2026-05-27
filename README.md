# 📊 Proyecto RappiPlus: De datos a decisiones de negocio

## 🧩 Introducción
RappiPlus es un servicio de suscripción dentro del ecosistema de Rappi diseñado para aumentar la frecuencia de compra y el valor generado por usuario.

Sin embargo, existen preguntas clave que requieren análisis:

- ¿Los usuarios realmente compran más?
- ¿El modelo está generando ganancias?
- ¿Se están perdiendo oportunidades en el proceso de compra?

Para responder estas preguntas, se trabaja con datos de pedidos, catálogo y marketing.  
El análisis permitirá entender el desempeño del servicio y detectar oportunidades concretas de mejora.

---

## 🎯 Objetivo del proyecto
A lo largo de este proyecto se responderán las siguientes preguntas:

- ¿Podemos confiar en los datos?
- ¿Estamos ganando dinero?
- ¿Dónde se pierden los usuarios?
- ¿Los usuarios regresan?
- ¿Los cambios generan impacto?
- ¿Cómo comunicamos todo esto?

---

## 🔄 Flujo del análisis

Cada etapa se construye sobre la anterior y responde una pregunta distinta del negocio.

### 📌 Pasos del análisis

| Paso | Pregunta clave                         | Resultado esperado                     |
|------|--------------------------------------|--------------------------------------|
| 1    | ¿Podemos confiar en los datos?        | Dataset limpio                        |
| 2    | ¿El negocio es rentable?              | KPIs (Revenue, Cost, Profit)         |
| 3    | ¿Dónde se pierden usuarios?           | Funnel de conversión                 |
| 4    | ¿Los usuarios regresan?               | Análisis de cohortes                 |
| 5    | ¿Los cambios funcionan?               | Test estadístico                     |
| 6    | ¿Cómo comunicamos los insights?       | Dashboard                            |

---

## 🔹 Paso 1: Preparación y calidad de datos (Python)

### 🎯 Objetivo
- Evaluar la calidad de los datos
- Detectar inconsistencias
- Limpiar y estructurar datasets
- Generar datos listos para análisis

### 📦 Entregable
- 3 datasets limpios

### 📂 Dataset del proyecto

El análisis comienza con tres fuentes principales:

- `rappiplus_orders_raw.csv`
- `rappiplus_catalog.csv`
- `rappiplus_marketing_spend.csv`

#### 📄 rappiplus_orders_raw.csv
Cada fila representa un pedido realizado en la plataforma.

#### 📄 rappiplus_catalog.csv
Cada fila representa un producto disponible en la plataforma.

#### 📄 rappiplus_marketing_spend.csv
Cada fila representa una inversión en marketing realizada por país y canal.

---

## 🔹 Paso 2: Análisis de rentabilidad del negocio (Python)

### 🎯 Objetivo
- Cálculo de KPIs:
  - Revenue (ingresos)
  - Cost (costos)
  - Profit (ganancias)
- Identificación de segmentos rentables

---

## 🔹 Paso 3: Análisis del funnel de conversión (SQL)

### 🎯 Objetivo
- Analizar el recorrido del usuario
- Construir el funnel completo
- Detectar puntos de abandono
- Identificar el mayor *drop-off*

### 🗂️ Fuente de datos
- Tabla `events`

---

## 🔹 Paso 4: Análisis de retención por cohortes (SQL)

### 🎯 Objetivo
- Analizar comportamiento en el tiempo
- Construir cohortes
- Obtener insights de retención

### 🗂️ Fuente de datos
- Tabla `users` → Información de registro de usuarios  
- Tabla `user_activity` → Actividad posterior al registro  

---

## 🔹 Paso 5: Evaluación de impacto (A/B Testing con Python)

### 🎯 Objetivo
- Analizar resultados del experimento
- Generar recomendaciones

### 🗂️ Fuente de datos
- `/datasets/experiment_checkout_ui.csv`  
Cada fila representa la participación de un usuario en un experimento A/B.

---

## 🔹 Paso 6: Dashboard y comunicación de insights

### 🎯 Objetivo
- Traducir análisis en visualizaciones
- Comunicar insights de forma clara
- Utilizar datasets limpios generados en el Paso 1

### 📦 Entregable
- Dashboard final

---

## 🚀 Resultado esperado

Al finalizar el proyecto se contará con:

- Datos confiables y limpios
- Métricas claras de negocio
- Identificación de oportunidades de mejora
- Evidencia estadística para toma de decisiones
- Visualizaciones listas para stakeholders

<p align="center">
  <img src="Vista_General_.png" width="700">
</p>

<p align="center">
  <img src="Vista_Detalle_.png" width="700">
</p>
