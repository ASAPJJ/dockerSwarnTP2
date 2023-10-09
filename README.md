#### Comandos para Crear Imágenes Docker:
- Crear imagen del servidor Apache:
  
  
  docker build -t image_apache ./apache-datos
  

- Crear imagen del servidor Node:
  

  docker build -t image_node ./node-datos
  

#### Comando para Desplegar Servicios con Docker Swarm:
- Utiliza el archivo "docker-compose.yml" para configurar el despliegue y ejecuta:
  

  docker stack deploy -c docker-compose.yml services


#### Acceso a los Servicios:
- Servicio de Apache: http://localhost:8080
- Servicio de Node: http://localhost:8090

#### Comandos para Borrar Servicios:
- Borrar servicio de Node:
  
  docker service rm services_node


- Borrar servicio de Apache:


  docker service rm services_apache


- Borrar servicio de la base de datos:


  docker service rm services_mysql
