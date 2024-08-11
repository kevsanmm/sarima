Análisis de Tendencias Climáticas y Medioambientales
Descripción del Proyecto
Este proyecto realiza un análisis exhaustivo de tendencias climáticas y medioambientales utilizando datos obtenidos a través de la biblioteca Pytrends, una API no oficial para Google Trends. El proyecto incluye la predicción del nivel del mar mediante un modelo SARIMAX y la verificación de la estacionariedad de diversas series temporales.

Datos
Los datos de este proyecto fueron obtenidos usando Pytrends, una herramienta que permite acceder a los datos de búsqueda en Google Trends. Pytrends proporciona acceso a datos de tendencias de búsqueda en varios países y permite explorar el interés de búsqueda en temas específicos a lo largo del tiempo. Los datos se agrupan en varias categorías como nivel del mar, temperaturas, dióxido de carbono y calentamiento global.

Modelos Utilizados
Modelo SARIMAX (Seasonal ARIMA with Exogenous Variables): Se utilizó este modelo para predecir el nivel del mar. El modelo configurado es ARIMA(5,1,0) con términos estacionales para capturar la estacionalidad anual. La validación del modelo mostró buenos ajustes según AIC, BIC y HQIC.

Pruebas de Estacionariedad: Se realizaron pruebas ADF (Dickey-Fuller aumentada) para verificar la estacionariedad de las series temporales de nivel del mar, temperaturas, dióxido de carbono y calentamiento global. Todas las series resultaron ser estacionarias.

Resultados y Conclusiones
El modelo SARIMAX proporciona predicciones confiables para el nivel del mar basado en los datos actuales.
Se observó heteroscedasticidad en los residuos del modelo, lo cual podría afectar la precisión de las predicciones futuras.
La inclusión de variables exógenas adicionales podría mejorar el modelo y su capacidad predictiva.
Instrucciones para Ejecutar el Código
Clona este repositorio: git clone https://github.com/kevsanmm/microdesafio7
Instala las dependencias necesarias: pip install -r requirements.txt
Configura tu entorno local con las credenciales necesarias para la base de datos, y asegúrate de que tu archivo de configuración .env esté configurado correctamente para conectar con tu base de datos.
Climate and Environmental Trends Analysis
Project Description
This project performs an in-depth analysis of climate and environmental trends using data sourced through the Pytrends library, an unofficial API for Google Trends. The project includes predicting sea level using a SARIMAX model and verifying the stationarity of various time series.

Data
The data for this project was obtained using Pytrends, a tool that provides access to Google Trends search data. Pytrends allows for querying search interest over time on specific topics and offers data for multiple countries. The data includes categories such as sea level, temperatures, carbon dioxide, and global warming.

Models Used
SARIMAX Model (Seasonal ARIMA with Exogenous Variables): This model was used to predict sea level. The configuration is ARIMA(5,1,0) with seasonal terms to capture annual seasonality. Model validation showed good fit according to AIC, BIC, and HQIC statistics.

Stationarity Tests: ADF (Augmented Dickey-Fuller) tests were conducted to check the stationarity of time series for sea level, temperatures, carbon dioxide, and global warming. All series were found to be stationary.

Results and Conclusions
The SARIMAX model provides reliable predictions for sea level based on current data.
Residuals showed heteroscedasticity, which could affect future prediction accuracy.
Exploring the inclusion of additional exogenous variables might enhance the model's predictive power.
Instructions to Run the Code
Clone this repository: git clone https://github.com/kevsanmm/microdesafio7
Install required dependencies: pip install -r requirements.txt
Configure your local environment with the necessary database credentials, ensuring that your .env file is set up correctly to connect to your database.
