# Análisis Espacial de Casos de COVID-19 en Perú (2020-2024) - [Tarea 4](https://yharaaa.github.io/Tarea-4/)

## Introducción y Fuente de Datos
Este análisis utiliza datos de casos positivos de COVID-19 proporcionados por el Ministerio de Salud de Perú (MINSA) a través de su plataforma de datos abiertos. [Enlace a la base de datos](https://www.datosabiertos.gob.pe/dataset/casos-positivos-por-covid-19-ministerio-de-salud-minsa). 

## Metodología

1. **Periodo de Análisis:** Se analizaron los datos entre 2020 y 2024, con un enfoque específico en el año 2021.

2. **Distribución Geográfica:** Utilizamos datos geográficos a nivel de departamento y provincia, integrados mediante geopandas para visualizar los casos de COVID-19 en mapas de Perú.

3. **Índice de Moran:** Calculamos el índice de Moran global, que reveló una débil autocorrelación espacial positiva (\(I = 0.17\)), sugiriendo que áreas con altas (o bajas) tasas de casos tienden a estar cerca, pero esta relación no es fuerte.

4. **Análisis LISA:** Identificamos patrones locales de autocorrelación:
   - **HH (Alto-Alto):** Clusters de alta incidencia, posibles focos de contagio.
   - **LL (Bajo-Bajo):** Zonas de baja incidencia.
   - **HL (Alto-Bajo) y LH (Bajo-Alto):** Outliers espaciales, áreas con tasas opuestas a sus vecinas.
   - **Visualización de Clusters:** Los mapas LISA ayudan a ubicar espacialmente estas áreas críticas para la toma de decisiones de salud pública.

5. **LISA Bivariado:** Evaluamos la relación espacial entre los casos de COVID-19 en 2021 y 2022, identificando áreas donde la incidencia se mantuvo alta (HH) o baja (LL), lo cual es útil para estrategias de salud pública enfocadas en reducir la transmisión.

## Visualización
### Moran Scatterplot y Mapas de Clusters
- Gráficos y mapas detallan la intensidad de los casos y la agrupación de valores altos y bajos a nivel provincial.

#### Gráficos

3. Índice de Moran
   
![image](https://github.com/user-attachments/assets/990372d8-cf53-49bc-904c-789ee4644ccf)


5. Análisis LISA
   
![image](https://github.com/user-attachments/assets/01cce74b-01c0-480f-9b21-71e144cdcccc)


6. LISA Bivariado
   
![image](https://github.com/user-attachments/assets/a69ee4dd-8780-450c-a24f-a09c591bd046)

