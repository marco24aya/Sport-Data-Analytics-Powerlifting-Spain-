# Análisis de datos AEP Powerlifting

## INTRODUCCIÓN

El presente trabajo consiste en la recapitulación del deporte de fuerza Powerlifting a nivel nacional en 2025. El powerlifting es un deporte de fuerza que consta de levantar el máximo peso en tres movimientos (Sentadilla, Press Banca y Peso Muerto) con tres intentos. El sistema actual de puntuaje son los GL Points, institucionalizado por la Federación Internacional de Powerlifting (IPF) desde 2022. 

## ¿Qué contiene?

En este repositorio contiene el CSV limpio y completo de las competiciones realizadas en España durante el 2025 y un CSV con los registros de los récords conseguidos durante la temporada. NO se incluyen competiciones continentales ni internacionales (eso lo dejo para un futuro). Los datos que hay son los mismos que los del primer repositorio, la novedad es que incluyo las provincias y Comunidades Autónomas de los clubs. Por último incluyo un Dashboard creado en PowerBI, donde he creado unas medidas, además de filtrados básicos para aportar información en las tarjetas. 

##  RESUMEN Análisis del Powerlifting
### ATLETAS

Comenzando el análisis, la participación en los campeonatos ha sido con una predominancia de los hombres, donde representa el 71% frente al 29% de las mujeres. La mayoría de los atletas se concentra en el rango de 24 a 39 años (45,54%), seguido de los Junior [18 - 24 años] con un 38,29% y los SubJuniors representan un 10%, en cuanto a los Másters (I - IV) su representación es inferior al 7%.

_Porcentaje y Distribución de la edad de los atletas_

<img width="562" height="474" alt="image" src="https://github.com/user-attachments/assets/ac5a99d6-b1e0-4d39-8ebd-aa9446c19d0b" />

<img width="1160" height="546" alt="image" src="https://github.com/user-attachments/assets/89896397-1e1a-4534-bca4-ab7f6725b967" />

Relacionado con la categoría de peso, los datos muestran que las categorías medias masculinas y femeninas son las más comunes entre los atletas. La categoría de **-83** es la predominante (20,3%) tanto en el caso masculino como en general. Le siguen -93 (17,1%) y -74 (12%). En el caso de las mujeres la categoría **-63** ocupa el primer puesto en las mujeres, y representa el 7,3% de entre todas las categorías, le siguen -69 y -59. Lo más reseñable es que las categorías ligeras y pesadas en ambos sexos no tienen mucha representación (>6%). 

####RENDIMIENTO DE ATLETAS

Para el rendimiento de un atleta en este deporte tiene un método llamado GL Points, implementadas en 2018 en competiciones internacionales, y que en 2022 fue implentado en España. Según IPF, su justificación se debe a que la método anterior no era justa ni equilibrada para todos los levantadores. 

Por lo que a este proyecto se refiere, me he querido centrar en primer lugar sobre los atletas con mayor GL Points, cuyo primer puesto lo ocupa UNA atleta con 111,95 GL Points, seguido de un atleta masculino con 110,06 GL Points. Inma Ruiz aparece ocupa los dos primeros puestos en el TOP 10 femenino, mientras que en el caso masculino hay una gran variedad de atletas, pero no de clubes, donde RV Strerngth y Berserkers son los que predominan el TOP. 

|                                                                #TOP 10 FEMENINO                                                         |
| Atleta                         | Cat peso | Cat edad | Club                | Total | Gl PTS | Competición                              |
|--------------------------------|----------|----------|---------------------|-------|--------|------------------------------------------|
| Soto Ruiz Inmaculada           | -63      | SNR      | LIFT AMBITION       | 510.5 | 111.95 | Campeonato de España Absoluto            |
| Soto Ruiz Inmaculada           | -69      | SNR      | LIFT AMBITION       | 495.5 | 107.33 | Copa de España Absoluto                  |
| Águila Padilla Ana María       | -57      | SNR      | BASIC STRENGTH      | 442.5 | 104.12 | Campeonato de España Absoluto            |
| Maguregi Rodríguez Jone        | -63      | SNR      | THE PR MODE         | 471.5 | 103.31 | Copa de España Absoluto                  |
| Prandi Merino Elsa             | -63      | JUN      | SPECIFIC STRENGTH   | 468.0 | 103.29 | Campeonato de España Junior              |
| González Molina Cristina       | -63      | JUN      | RV STRENGTH         | 470.5 | 103.23 | Campeonato de España Junior              |
| Ormaetxea Prieto Leire         | -57      | JUN      | GOIERRI KE          | 435.0 | 102.09 | I Campeonato de Euskal Herria            |
| Maguregi Rodríguez Jone        | -63      | SNR      | THE PR MODE         | 462.5 | 102.07 | Campeonato de España Absoluto            |
| Veiga Lestegas Rosalía         | -69      | SNR      | 720 POWERLIFTING    | 484.0 | 101.98 | Campeonato de España Absoluto            |
| Sarría Pascual Alba            | -63      | SNR      | THE NEW ERA         | 457.5 | 101.60 | II SBD Cup                               |


|                                                                #TOP 10 MASCULINO                                                               |
| Atleta                                 | Cat peso | Cat edad | Club                     | Total | GL PTS | Competición                         |
|----------------------------------------|----------|----------|--------------------------|-------|--------|-------------------------------------|
| Pérez Barros Antonio                   | -105     | SNR      | BASIC STRENGTH           | 889.0 | 110.06 | Campeonato de España Absoluto       |
| Fernández Arévalo Andrés               | -83      | JUN      | BERSERKERS               | 785.5 | 110.05 | Campeonato de España Junior         |
| Montano Camacho Mario                  | -93      | SNR      | RV STRENGTH              | 825.0 | 108.24 | Campeonato de España Absoluto       |
| Fernández Arévalo Andrés               | -83      | JUN      | BERSERKERS               | 775.0 | 107.96 | Campeonato de España Absoluto       |
| El Moukallif Naim Ali                  | -83      | JUN      | FORÇA VILAFRANCA          | 762.5 | 106.90 | Campeonato de España Absoluto      |
| Souto Romero Marcos                    | -83      | JUN      | SPECIFIC STRENGTH        | 765.0 | 105.95 | Campeonato de España Absoluto       |
| Herraiz Francés Alberto                | -74      | SNR      | BERSERKERS               | 717.5 | 105.54 | Campeonato de España Absoluto       |
| Souto Romero Marcos                    | -83      | JUN      | SPECIFIC STRENGTH        | 760.0 | 105.34 | I Campeonato Intend Power           |
| Pérez Nova José                        | -93      | JUN      | POWERLIFTING ALBACETE    | 802.5 | 105.29 | Campeonato de España Absoluto       |
| Vázquez Hernández-Carrillo Víctor      | -120     | SNR      | RV STRENGTH              | 892.5 | 104.24 | Campeonato de España Absoluto       |


|                                                                #TOP Atletas en cada movimiento                                                           |
| Sexo| Movimiento | Atleta                                 | Cat peso | Cat edad | Club                     | KGS   | Competición                         |
|-----|------------|----------------------------------------|----------|----------|--------------------------|-------|-------------------------------------|
|M    | Sentadilla | Pérez Barros Antonio                   | -105     | SNR      | BASIC STRENGTH           | 889.0 | Campeonato de España Absoluto       |
|F    | Sentadilla | Sánchez Jorge Carla                    | -84      | JUN      | ATENEA                   | 202.5 | Campeonato de España Junior         |
|M    | Press Banca | Ardenghi Teira Gianluca               | >120     | JUN      | ATLETAS FUERZA CASARICHE | 220.0 | XI Campeonato Sur                   |
|F    | Press Banca | Prandi Merino Elsa                    | -63      | JUN      | SPECIFIC STRERNGTH       | 115.0 | Campeonato de España Junior         |
|M    | Peso Muerto | Pérez Barros Antonio                  | -105     | SNR      | BASIC STRENGTH           | 363.5 | Campeonato de España Absoluto       |
|F    | Peso Muerto | Erimo Sabadell Rosa                   | -84      | SNR      | RV STRENGTH              | 225.5 |  Campeonato de España Absoluto      |






**DASHBOARD**
<img width="1281" height="721" alt="image" src="https://github.com/user-attachments/assets/447bf673-9078-4ace-952d-1a82965ed901" />

## FINALIDAD
Con este poryecto he querido demostrar mis capacidades técnicas con el uso de Excel para la recopilación de datos, donde he podido utilizar algunas funciones como  Python para realizar data cleaning, EDA, y con Power BI mi manera de transmitir la información más relevante del año 2025 en este deporte, además del uso de las diferentes visualizaciones y realizando alguna relación con diferentes tablas. Por otro lado, conviene resaltar que este proyecto tiene con fines didácticos y que no supone ninguna relación laboral con la AEP. 
