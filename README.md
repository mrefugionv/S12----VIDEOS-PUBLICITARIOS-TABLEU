# S12----VIDEOS-PUBLICITARIOS-TABLEU
Automatización de dashboard para resolución de preguntas frecuentes para equipo de publicidad sobre las categorías de videos más vistos. Tableu.

## Descripción
Trabajas como analista de vídeos publicitarios en la agencia de publicidad Sterling & Draper. Dedicas mucho tiempo a analizar tendencias de vídeos en YouTube para determinar qué contenido merece atención para la mercadotecnia.

Cada video tiene una categoría específica (entretenimiento, música, noticias y política, etc.), una región y una fecha en que se hace tendencia.

Un video puede estar en la sección de tendencias durante varios días seguidos.

Cada semana, las nuevas empleadas Melanie y Ashok te preguntan esto:

1. ¿Qué categorías estaban en las tendencias de la semana pasada?
2. ¿Cómo se distribuyeron en diversas regiones?
3. ¿Qué categorías fueron particularmente populares en los Estados Unidos?

En tu sexta semana en el trabajo, decides que ya es momento de que el proceso sea automático. Vas a crear un dashboard para Melanie y Ashok.

## Herramientas utilizadas
![Tableu](https://img.shields.io/badge/:Tableu-8C4966?style=for-the-badge&logo=microstrategy&logoColor=white&labelColor=101010)</br>
![Google Drive](https://img.shields.io/badge/Google%20Drive-4285F4?style=for-the-badge&logo=googledrive&logoColor=white)

Acceda al Dashboard en el servidor de Tableau Public mediante el link:
https://public.tableau.com/views/ProyectoS12_17477814824440/Dashboard1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

En el PDF anexo encontrara una presentación con las características técnicas del dashboard 
y una segunda sección con las respuestas a las cuestionas planteadas por el equipo de marketing.

## Conclusiones
1. Durante el periodo registrado 14/11/2017 - 14/06/2018 las categorías en más tendencia fueron:
   * Entretenimiento : Representó entre un 24 - 35 % de los vídeos cada día.
   * People & Blogs :  Representó entre 9 - 15 % de los vídeos cada día.
   * News  Politics: Representó entre 7 - 14 % de los vídeos cada día.
   * Music : Representó entre 6 - 14 % de los vídeos cada día.
   * Comedy : Representó entre 6 - 11 % de los vídeos cada día.
   Estas conclusiones se obtuvieron mediante el gráfico “Historial de tendencias, %” 

2. Durante el periodo registrado 14/11/2017 - 14/06/2018 se observa una distribución equitativa de registros entre las regiones de Francia(22.09%), Estados Unidos (23.68%), India (21.45%), Rusia (21.62%); únicamente Japón registra menor cantidad (11.16%).  Se descubre que esta diferencia se da por que hasta febrero del 2018 no se cuentan con registros de Japón.
Estas conclusiones se obtuvieron mediante el gráfico “Tendencias de video por país” .

3. Para la semana pasada 07/06/2018 - 14/06/2018 se observa en la tabla “Tendencias de video por país y por categoría”:
   Para E.E.U.U. fue particularmente popular  las categorías de ‘entretenimiento’ y ‘ música’.
   Prácticamente en todas las regiones la categoría más popular fue ‘entretenimiento’, excepto en Rusia que fue ‘People & Blogs’.


## Profundización técnica
* Creación de dashboard :
* * Diseño de dashboard en conjunto con el equipo que lo requiere :
  * * Objetivo de negocios: analizar el historial de tendencias de videos en YouTube
    * Con qué frecuencia se usará el dashboard: al menos una vez al día
    * Usuario objetivo del dashboard: gerentes de planificación de videos publicitarios
    * Contenido de los datos del dashboard:
    * * Tendencias pasadas de videos, ordenadas por día y categoría
      * Tendencias de videos, ordenadas por país
      * Una tabla de correspondencia entre categorías y países
    * Parámetros para agrupar los datos:
    * * Fecha y hora de tendencia
      * Categoría de video
      * País
    * Los datos:
    * * Historial de tendencias — valores absolutos ordenados por día (dos gráficos: números absolutos y proporción de porcentaje)
      * Eventos, ordenados por país — valores relativos (% de eventos)
      * La correspondencia entre las categorías y los países — valores absolutos (una tabla)
    * Importancia: todaos los gráficos son igualmente importantes
    * Fuentes de datos para el dashboard: los ingenieros prometieron crear una tabla de agregación llamada trending_by_time. Esta es la estructura:
    * * record_id: la clave primaria
      * region: país/región geográfica
      * trending_date fecha y hora
      * category_title categoría del video
      * videos_count número de videos en la sección de tendencias
