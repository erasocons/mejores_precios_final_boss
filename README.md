# mejores_precios_final_boss
Buscador inteligente de precios de la canasta familiar que compara productos según precio y ubicación, optimiza listas de compra y utiliza IA para encontrar productos, recomendar recetas y generar opciones según presupuesto.


Componentes principales
1. Motor de búsqueda

Permitirá buscar productos mediante:

Nombre.
Categoría.
Marca.
Presentación.
Código de producto.
Lenguaje natural.

Ejemplo:

"leche deslactosada barata cerca de mí"
2. Sistema de comparación

Comparará productos entre diferentes establecimientos teniendo en cuenta:

Precio.
Cantidad.
Unidad de medida.
Marca.
Presentación.
Ubicación.
Disponibilidad.
3. Sistema de geolocalización

Permitirá calcular:

Distancia al establecimiento.
Tiempo aproximado de desplazamiento.
Establecimientos cercanos.
Opciones dentro de un radio determinado.
4. Motor de recomendaciones

Generará recomendaciones considerando diferentes variables.

Precio
↓
Distancia
↓
Presupuesto
↓
Preferencias
↓
Disponibilidad
↓
Historial
↓
RECOMENDACIÓN
5. Inteligencia artificial

La IA funcionará como una interfaz conversacional sobre el sistema de búsqueda.

El usuario podrá escribir:

"Quiero preparar cinco almuerzos baratos esta semana."

La IA podrá convertir esa petición en:

Objetivo
↓
Número de comidas
↓
Ingredientes necesarios
↓
Productos disponibles
↓
Precios
↓
Ubicación
↓
Presupuesto
↓
Plan de compra
🏗️ Tecnologías

La arquitectura tecnológica podrá evolucionar durante el desarrollo.

Backend
Python
FastAPI
APIs REST
Procesamiento de datos
Data Engineering
Python
Pandas
ETL / ELT
Web scraping cuando sea permitido
APIs de establecimientos
Validación y normalización de datos
Base de datos

Posibles tecnologías:

PostgreSQL
PostGIS
Redis
Machine Learning / IA
Modelos de lenguaje (LLM)
Embeddings
Sistemas de recomendación
NLP
Clasificación de productos
Frontend

Posibles tecnologías:

React
Next.js
HTML/CSS/JavaScript
Infraestructura

Posibles servicios:

AWS
Docker
GitHub Actions
Servicios cloud para APIs y bases de datos
🗂️ Estructura inicial del proyecto
price-finder/
│
├── backend/
│   ├── api/
│   ├── services/
│   ├── models/
│   └── main.py
│
├── data/
│   ├── raw/
│   ├── processed/
│   └── external/
│
├── etl/
│   ├── extraction/
│   ├── transformation/
│   └── loading/
│
├── ai/
│   ├── prompts/
│   ├── recommendations/
│   └── search/
│
├── frontend/
│
├── notebooks/
│
├── tests/
│
├── docs/
│
├── requirements.txt
│
└── README.md
🗺️ Roadmap
Fase 1 — MVP

Base de datos inicial de productos.

Normalización de productos.

Motor de búsqueda.

Comparación de precios.

Interfaz básica.

Filtro por ciudad.

Fase 2 — Geolocalización

Ubicación del usuario.

Distancia a establecimientos.

Búsqueda por radio.

Comparación precio + distancia.

Fase 3 — Lista de mercado

Crear listas.

Calcular costo total.

Comparar establecimientos.

Optimizar combinación de tiendas.

Fase 4 — Inteligencia artificial

Búsqueda mediante lenguaje natural.

Interpretación de ingredientes.

Recomendación de productos.

Generación de recetas.

Recomendaciones basadas en presupuesto.

Fase 5 — Datos históricos

Historial de precios.

Estadísticas.

Detección de variaciones.

Identificación de precios inusualmente bajos o altos.

Fase 6 — Optimización

Personalización.

Recomendaciones avanzadas.

Optimización de rutas.

Predicción de precios.

Sistema de alertas.

🔬 Problemas técnicos interesantes

Este proyecto permite trabajar diferentes áreas de ingeniería y analítica de datos:

Data Engineering

Construcción de pipelines para recopilar, limpiar, transformar y almacenar precios.

Data Analytics

Análisis de:

Evolución de precios.
Diferencias regionales.
Inflación por categoría.
Productos con mayor variabilidad.
Diferencias entre establecimientos.
Machine Learning

Posibles aplicaciones:

Recomendación de productos.
Predicción de precios.
Detección de anomalías.
Clasificación automática de productos.
Predicción de demanda.
NLP / LLM

Interpretación de consultas como:

"Quiero hacer una cena barata para cuatro personas."

y convertirlas en búsquedas estructuradas.

Optimización

Encontrar la combinación de productos y establecimientos que minimice el costo total bajo diferentes restricciones.

🌎 Alcance inicial

El proyecto comenzará enfocado en Colombia, inicialmente en una ciudad determinada.

La arquitectura se diseñará para poder incorporar posteriormente:

Nuevas ciudades.
Nuevos establecimientos.
Nuevas categorías.
Nuevas fuentes de datos.
⚠️ Consideraciones sobre los datos

Los precios pueden cambiar constantemente y depender de:

Ciudad.
Establecimiento.
Fecha.
Disponibilidad.
Promociones.
Presentación.
Método de pago.

Por esta razón, el sistema deberá almacenar información temporal asociada a cada precio.

Producto
+
Establecimiento
+
Ubicación
+
Precio
+
Fecha/hora
+
Presentación

Esto permitirá diferenciar entre un precio actual y un precio histórico.

🚀 Visión del proyecto

La visión es evolucionar desde un simple:

"comparador de precios"

hacia un:

"asistente inteligente para comprar alimentos y productos de la canasta familiar".

El usuario no debería tener que saber qué producto buscar, en qué tienda buscarlo ni cómo comparar todas las alternativas.

Podría simplemente decir:

"Tengo $100.000, quiero hacer mercado para una semana y quiero cocinar comidas saludables."

y el sistema debería ser capaz de transformar esa intención en:

🛒 Lista de compras
+
💰 Precios
+
📍 Establecimientos
+
🚗 Distancias
+
🍳 Recetas
+
💵 Presupuesto
+
🤖 Recomendaciones

El objetivo final es convertir los datos de precios disponibles en una herramienta que ayude a las personas a tomar mejores decisiones de compra de manera rápida, contextualizada y basada en datos.

📄 Licencia

Este proyecto se encuentra actualmente en desarrollo.

La licencia será definida posteriormente
