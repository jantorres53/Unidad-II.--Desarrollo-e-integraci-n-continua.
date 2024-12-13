
# Lista de Comandos Docker

## Índice
1. [Docker Engine](#docker-engine)
2. [Docker Compose](#docker-compose)
3. [Docker Swarm](#docker-swarm)

---

## Docker Engine

### Comandos básicos:

- **Listar contenedores en ejecución:**  
```shell
docker ps
```

- **Listar todos los contenedores:**  
```shell
docker ps -a
```

- **Iniciar un contenedor detenido:**  
```shell
docker start <nombre_o_id_contenedor>
```

- **Detener un contenedor en ejecución:**  
```shell
docker stop <nombre_o_id_contenedor>
```

- **Eliminar un contenedor:**  
```shell
docker rm <nombre_o_id_contenedor>
```

- **Eliminar una imagen:**  
```shell
docker rmi <id_imagen>
```

- **Inspeccionar un contenedor:**  
```shell
docker inspect <nombre_o_id_contenedor>
```

- **Ver estadísticas de uso de recursos de contenedores:**  
```shell
docker stats
```

---

## Docker Compose

### Comandos básicos:

- **Iniciar contenedores definidos en `docker-compose.yml`:**  
```shell
docker-compose up
```

- **Detener contenedores y servicios definidos:**  
```shell
docker-compose down
```

- **Ver logs de servicios:**  
```shell
docker-compose logs
```

- **Recrear contenedores:**  
```shell
docker-compose up --force-recreate
```

- **Construir imágenes sin iniciar contenedores:**  
```shell
docker-compose build
```

- **Escalar servicios:**  
```shell
docker-compose up --scale <servicio>=<número>
```

---

## Docker Swarm

### Comandos básicos:

- **Inicializar Docker Swarm:**  
```shell
docker swarm init
```

- **Unirse a un clúster Swarm existente:**  
```shell
docker swarm join --token <token> <ip>:<puerto>
```

- **Listar nodos del clúster:**  
```shell
docker node ls
```

- **Salir del clúster Swarm:**  
```shell
docker swarm leave
```

- **Crear un servicio:**  
```shell
docker service create --name <nombre_servicio> <imagen>
```

- **Listar servicios en el clúster:**  
```shell
docker service ls
```

- **Actualizar un servicio:**  
```shell
docker service update <opciones> <nombre_servicio>
```

- **Eliminar un servicio:**  
```shell
docker service rm <nombre_servicio>
```

