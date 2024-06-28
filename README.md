
# Análisis y Modelado de Dataset de Empleados

## Descripción del Proyecto
Este proyecto desarrolla el análisis y modelado sobre un dataset de empleados de una empresa. El dataset incluye información sobre la educación, año de incorporación, ciudad de trabajo, categoría salarial, edad, género, si han sido asignados temporalmente a la banca (EverBenched), experiencia en el dominio actual y si el empleado tomó tiempo libre (LeaveOrNot). El dataset ha sido modificado para incluir datos faltantes, añadiendo realismo al desafío analítico.

## Ejecución
Para ejecutar este proyecto, sigue los siguientes pasos:

1. Clona este repositorio:
   ```bash
   git clone <URL_del_Repositorio>
   cd <Nombre_del_Repositorio>
   ```

2. Instala las dependencias necesarias:
   ```bash
   pip install pandas matplotlib scikit-learn
   ```

3. Abre el notebook `Analisis_y_Prediccion_de_Datos_de_Empleados.ipynb` en Jupyter Notebook o Jupyter Lab y ejecuta cada celda para realizar el análisis y modelado.

## Resumen del Análisis
- **Preprocesamiento de Datos**: Se manejaron valores faltantes mediante la eliminación de filas con valores críticos faltantes y la imputación de datos en las columnas `Age` y `PaymentTier`. También se eliminaron valores atípicos basados en el análisis de IQR.
- **Análisis Exploratorio de Datos**: Se realizaron visualizaciones para entender la distribución de géneros y niveles de educación. Además, se exploró la relación entre la edad y la probabilidad de tomar licencias.
- **Modelado de Datos**: Se entrenaron dos modelos de RandomForest (uno sin balanceo de clases y otro con balanceo de clases). Se evaluaron sus rendimientos en términos de accuracy y F1 score, y se presentaron matrices de confusión para una mejor comprensión del rendimiento de los modelos.

## Conclusiones
El análisis y modelado del dataset de empleados permitió obtener varias conclusiones importantes:
- La distribución de género en la empresa está equilibrada, con una ligera mayoría de un género sobre otro.
- Los niveles de educación presentan una distribución variada, siendo algunos niveles más comunes que otros.
- La edad de los empleados tiene una relación interesante con la probabilidad de tomar licencias, destacando ciertos grupos etarios.
- Los modelos de RandomForest utilizados demostraron que el balanceo de clases puede mejorar significativamente el rendimiento en datasets desbalanceados, proporcionando una mayor precisión y un mejor F1 score.
