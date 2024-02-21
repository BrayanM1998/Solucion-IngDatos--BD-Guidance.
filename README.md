# SOLUCION PRUEBA ING DATOS - BD GUIDANCE

# Inicializar los contenedores con Docker

Para el acceso a la base de datos dvdrental se establecio inicialmnete una conexecion mediante el programa Docker, siguiendo las intrucciones planteadas

    
    cd data_warehouse
    docker build -t imagen_dw_dvdrental .
    docker run -d --net dw_network -p 5431:5432 --name dw_dvdrental_contenedor imagen_dw_dvdrental
    
    

## Data Ware House
   #### Modelo Estrella
![dw_dvdrental -Modelo Estrella- public](https://github.com/BrayanM1998/Solucion-IngDatos--BD-Guidance./assets/160368046/285ab87f-59aa-475b-9f90-bf402bfe2449)
   #### Almacen de Datos
![Captura de pantalla (14)](https://github.com/BrayanM1998/Solucion-IngDatos--BD-Guidance./assets/160368046/29a2707a-ef7f-47f4-a64e-738c8da22139)

Para la creacion del Data WareHouse  implemente el lenguaje de programacion python con el entorno de 'Jupyter Notewook' para realizar las siguientes tareas:
  - Crear tablas DW: En esta creo la estructura que va a tener cada una de mis tablas en el dw, estableciendo de tal menera el modelo fisico de estrella de mmi base de datos DW
  - Carga ETL DW: En este apartado genero toda la transformacion requerida para la carga de los datos requeridos
    ![etl](https://github.com/BrayanM1998/Solucion-IngDatos--BD-Guidance./assets/160368046/23b2af68-37bb-468c-b7d5-c5b2be1bdba7)

  - Eliminacion tablas DW: En este script se borran las tablascontenidas en el DW de tal menera que me permita nuavenete retroalimentar el DW desde la base de datos transaccional, en caso de ser requerido

### Solucion

-  Aqui genero dos archivos de jupyter notework en donde se resulven cada uno de los objetivos planteados: tanto en la base de datos transaccional (original) como el Data Were House Original
  ![solucion](https://github.com/BrayanM1998/Solucion-IngDatos--BD-Guidance./assets/160368046/1da0cbc8-0b1d-412f-926f-fbed9ffdd127)

#### Nota:De ser necesario, tambien realice el backup del Data Ware House (Se encunta dentro de la carpeta). Importante tambien mencionar que en los archivos de jupyter se muestra una previsualizacion de los resultados obtenidos en cada ejecucion

## Dash Board

Aqui se implemto el panel de control, dando solucion de manera grafica y estadistica a cada uno de los objetivos planteados. 

#### Conectando directanete el Data Ware House realizado. Para la visualizacion y presenytacion de archivos
![powerbi](https://github.com/BrayanM1998/Solucion-IngDatos--BD-Guidance./assets/160368046/ea8d3e3d-48e9-4156-ac96-d6bd8f21931e)
