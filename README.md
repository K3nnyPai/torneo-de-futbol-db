# Base de Datos Torneo Deportivo

Este repositorio contiene las colecciones exportadas de MongoDB en formato JSON para la gestión de un torneo de futbol deportivo.

## Estructura del Repositorio

- `deportistas.json`: Información de los deportistas registrados.
- `encuentros.json`: Información de los encuentros deportivos que tiene cada equipo.
- `entrenadores.json`: Datos de los entrenadores.
- `arbitros.json`: Información de los árbitros asignados.
- `equipos.json`: Equipos participantes.
- `tabla_posiciones.json`: Tabla de posiciones actualizada.

## Cómo usar

1. Descargue los archivos `json` o clonarlos tambien es una buena opción

2. Importa las colecciones en tu instancia de MongoDB:
   ```bash
   mongoimport --db torneo --collection deportistas --file deportistas.json
   mongoimport --db torneo --collection entrenadores --file entrenadores.json
   mongoimport --db torneo --collection arbitros --file arbitros.json
   mongoimport --db torneo --collection equipos --file equipos.json
   mongoimport --db torneo --collection tabla_posiciones --file tabla_posiciones.json

2.1 o podemos importarlas tambien desde mongoDBCompass:

 - Abrimos mongoDB y creamos una base de datos llamada `champions`
 - Creamos las colecciones: `arbitros`, `deportistas`, `encuentros`, `entrenadores`, `equipos`, `tabla_posiciones`
 - Una vez creadas las colecciones nos dirigimos a una y le daremos en la opcion `import data`
![image](https://github.com/user-attachments/assets/0c875805-9b39-48b4-8691-bb8e33ff0ae1)
- Seleccionamos el archivo json que tiene la coleccion creada, es decir, si creamos la coleccion `arbitros` seleccionamos el archivo `arbitros.json` y asi con todas las colecciones

