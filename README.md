Proyecto Final de Business Intelligence — Análisis de Ventas Farmacéuticas

Este repositorio contiene el desarrollo completo del proyecto final de Business Intelligence aplicado a un caso de análisis de ventas en una farmacia.
Incluye el pipeline ETL, análisis exploratorio EDA, KPIs, visualizaciones y un dashboard interactivo en Streamlit.

Objetivo del Proyecto

Construir un proceso completo de Business Intelligence que permita:

Analizar más de 30,000 transacciones de una farmacia.

Detectar las categorías y productos más rentables.

Identificar tendencias temporales de compra.

Construir un dashboard para la toma de decisiones.

Documentar el flujo ETL para garantizar reproducibilidad.

Instalación y Configuración
1. Clonar el repositorio
   
git clone https://github.com/LuisMario87/ProyectoPreliminarBI.git
cd ProyectoPreliminarBI

2. Instalar dependencias
pip install -r requirements.txt

Pipeline ETL

El ETL se encuentra en:

scripts/EtlFinal.py
Incluye:

Extract: lectura del archivo RAW.

Transform: limpieza, formateo, tipos de dato, cálculo de TotalVenta.

Data Quality Report: nulos, duplicados y estadísticas.

Load: exportación del dataset procesado para análisis.

Ejecutarlo:

python scripts/EtlFinal.py

Notebook de Análisis

Disponible en:

notebook/notebook.ipynb

Incluye:

KPIs con fórmulas.

Gráficas avanzadas:

Ventas por categoría

Ventas semanales

Top 5 productos más vendidos

Heatmap día-mes

Interpretación narrativa de cada visualización.

Preparación previa al dashboard.

Dashboard en Streamlit

Código ubicado en:

notebook/dashboard.py


Ejecutarlo localmente:

streamlit run dashboard/app.py


Incluye:

Filtros interactivos

Gráficas dinámicas

Resumen de KPIs

Exploración de patrones en tiempo real

Limitaciones

Dataset con nombres ficticios y ciudades generadas sintéticamente.

Ausencia de costos operativos (no se puede analizar margen).

No contiene datos personales por motivos de anonimización.

No es posible calcular métricas avanzadas como recurrencia sin historial consolidado.

Recomendaciones

Integrar datos contables para medir rentabilidad real.

Registrar campañas de marketing para relacionarlas con peaks de ventas.

Implementar un modelo de predicción para estimar demanda futura.

Añadir alertas automáticas de inventario usando el mismo pipeline de BI.

Conclusión

Este proyecto demuestra cómo construir un sistema completo de Business Intelligence capaz de transformar datos crudos en conocimiento útil, aplicando un flujo profesional de ETL, análisis exploratorio, visualización y dashboard interactivo.

Contacto

Luis Mario Ayala Castellanos
📧 luis.ayalacr@udlap.mx
