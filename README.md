# Colombianos SIN FRONTERAS

**Descripción**  
"Colombianos SIN FRONTERAS" es una aplicación creada con Streamlit para visualizar y analizar datos sobre la diáspora colombiana en el mundo. Esta plataforma proporciona acceso a información de una base de datos SQL Server, presenta filtros de datos personalizados y gráficos interactivos, y ofrece una experiencia de usuario envolvente mediante el uso de animaciones y elementos visuales personalizados.

## Funcionalidades

### 1. Conexión a Base de Datos
- **Función `obtener_datos`**: Realiza la conexión a una base de datos SQL Server para obtener los datos de los colombianos en el exterior. Incluye manejo de errores y muestra un mensaje de éxito en caso de conexión exitosa.
- **Consulta SQL**: Ejecuta una consulta que selecciona los primeros 250,000 registros para análisis.

### 2. Visualización de Animaciones Lottie
- **Función `load_lottie_url`**: Carga animaciones Lottie a partir de una URL para hacer la aplicación más interactiva y visualmente atractiva.
- **Lottie Animation**: Muestra una animación de bienvenida que mejora la experiencia visual del usuario.

### 3. Páginas de Navegación
- **Página de Bienvenida**: Introduce la aplicación, muestra la animación de bienvenida y registra el tiempo de permanencia en la página.
- **Página de Datos**: Muestra los datos obtenidos de la base de datos, permite aplicar filtros, y presenta gráficos para un análisis detallado.

### 4. Filtros Dinámicos
Permite a los usuarios filtrar datos según tres criterios: 
  - **País**
  - **Género**
  - **Grupo de Edad**

Estos filtros ayudan a personalizar y refinar los datos visibles en la tabla y los gráficos.

### 5. Visualización Interactiva con Gráficos
- **Gráfico de Barras**: Muestra la distribución de personas registradas por país y género.
- **Gráfico de Dispersión**: Representa la relación entre la edad y la estatura de los individuos.
- **Sidebar de Opciones de Visualización**: 
  - Permite al usuario seleccionar una columna y tipo de gráfico (Histograma, Gráfico de Barras, o Gráfico de Dispersión).
  - **Histograma**: Visualiza la distribución de valores de una columna.
  - **Gráfico de Barras**: Muestra la frecuencia de valores en una columna específica.
  - **Gráfico de Dispersión**: Permite la comparación entre dos columnas de datos.

### 6. Mapa Interactivo
- **Ubicaciones en Mapa**: Visualización de todas las ubicaciones geográficas (latitud y longitud) en un mapa interactivo que muestra la distribución global de la diáspora colombiana.

### 7. Resumen Estadístico
- **Resumen Descriptivo**: Al activar esta opción, se genera un resumen estadístico de los datos disponibles.

## Configuración del Entorno

### Requisitos
- Python 3.8 o superior.
- Las siguientes bibliotecas de Python:
  - `streamlit`
  - `pandas`
  - `pyodbc`
  - `altair`
  - `folium`
  - `plotly`
  - `requests`
  - `numpy`
  - `streamlit-folium`
  - `streamlit-lottie`
  - `streamlit-globe`

### Configuración de Base de Datos
Para la conexión a SQL Server, asegúrate de tener:
- **Nombre del Servidor**: `"DESKTOP-F80T3P0\\SQLEXPRESS"`
- **Base de Datos**: `"ColombianosExterior_bd"`
- **Usuario y Contraseña**: `"support"`, `"sdu2024"`
  
Ajusta los detalles de la conexión según tu entorno si estos parámetros cambian.

---

Este README proporciona una guía completa de las funcionalidades y configuraciones para utilizar "Colombianos SIN FRONTERAS" y permite aprovechar al máximo las capacidades interactivas de análisis de datos y visualización de la diáspora colombiana.


