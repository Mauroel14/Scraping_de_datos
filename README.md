# RPA Bot: Automatización de Consultas de Facturación y Deuda 🤖💸

## 📝 Descripción del Proyecto
Este proyecto es una solución de **Robotic Process Automation (RPA)** desarrollada en Python. El objetivo principal es automatizar el proceso de consulta de facturas impagas en el portal **PowerCRM de Movistar**. 

El bot reemplaza una tarea manual repetitiva, permitiendo procesar cientos de líneas telefónicas de forma masiva, extrayendo montos de deuda y consolidando la información en un reporte estructurado.

## 🚀 Características Principales
* **Navegación Autónoma:** Inicio de sesión automático, manejo de menús dinámicos y navegación por el árbol de la plataforma CRM.
* **Procesamiento Masivo:** Integración con archivos Excel (`pandas`) para procesar múltiples registros en un solo ciclo.
* **Web Scraping Avanzado:** Extracción de datos en tiempo real desde elementos dinámicos del DOM utilizando Selenium.
* **Gestión de Errores y Logs:** Sistema de captura de excepciones para identificar líneas sin factura o errores de carga, registrando cada evento en un archivo `.csv`.

## 🛠️ Stack Tecnológico
* **Lenguaje:** Python
* **Automatización:** Selenium WebDriver
* **Análisis de Datos:** Pandas (para manejo de Excel y CSV)
* **Control de Navegador:** Chrome WebDriver

## 📁 Estructura del Repositorio
* `bot_facturacion.py`: Script principal con la lógica de automatización.
* `lineas.xlsx`: Archivo de entrada donde se deben colocar los números de línea a consultar.
* `datosFacturaImpaga.csv`: Reporte de salida generado automáticamente con el formato `Línea, Monto/Error`.

## ⚙️ Configuración e Instalación

1. **Requisitos Previos:**
   * Python 3.x instalado.
   * Google Chrome instalado.
   * `chromedriver.exe` en la raíz del proyecto (debe coincidir con tu versión de Chrome).

2. **Instalación de Librerías:**
   ```bash
   pip install selenium pandas openpyxl
