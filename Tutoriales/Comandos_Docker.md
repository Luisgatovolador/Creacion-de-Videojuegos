
# Lista de Comandos Docker

> **Universidad Tecnológica del Norte de Guanajuato**  
> **Carrera:** Ingeniería en Desarrollo y Gestión de Software  
> **Materia:** Gestión del Proceso de Desarrollo de Software ING  
> **Profesor:** Eric Domenzain Morales 
> **Autor:** Rodríguez López Luis Oswaldo  
> **Grupo:** GIDS5103  
---

## Índice

1. [Docker Engine](#docker-engine)
   - [Imágenes](#imágenes)
   - [Contenedores](#contenedores)
   - [Control de contenedores](#control-de-contenedores)
   - [Logs y monitoreo](#logs-y-monitoreo)
   - [Interacción con contenedores](#interacción-con-contenedores)
   - [Limpieza](#limpieza)
2. [Docker Compose](#docker-compose)
3. [Docker Swarm](#docker-swarm)
4. [Ejemplo de uso práctico](#ejemplo-de-uso-práctico)

---

## Docker Engine

### Imágenes

**Lista todas las imágenes descargadas en tu sistema**
```shell
docker images
````

**Descarga una imagen desde Docker Hub**

```shell
docker pull <imagen>
```

**Elimina una imagen del sistema**

```shell
docker rmi <id_imagen>
```

**Busca imágenes en Docker Hub**

```shell
docker search <nombre>
```

---

### Contenedores
         
**Muestra los contenedores en ejecución**

```shell
docker ps
```

**Lista todos los contenedores (activos e inactivos)**

```shell
docker ps -a
```

**Crea e inicia un contenedor a partir de una imagen**

```shell
docker run <imagen>
```

**Inicia un contenedor en segundo plano**

```shell
docker run -d <imagen>
```

**Mapea puertos entre el host y el contenedor**

```shell
docker run -d -p <puerto_host>:<puerto_contenedor> <imagen>
```

**Crea un contenedor con un nombre específico**

```shell
docker run --name <nombre_contenedor> <imagen>
```

---

### Control de contenedores

**Inicia un contenedor detenido**

```shell
docker start <id_contenedor>
```

**Detiene un contenedor en ejecución**

```shell
docker stop <id_contenedor>
```

**Reinicia un contenedor**

```shell
docker restart <id_contenedor>
```

**Elimina un contenedor detenido**

```shell
docker rm <id_contenedor>
```

**Elimina todos los contenedores detenidos**

```shell
docker container prune
```

---

### Logs y monitoreo

**Muestra los logs de un contenedor**

```shell
docker logs <id_contenedor>
```

**Muestra los logs en tiempo real**

```shell
docker logs -f <id_contenedor>
```

**Muestra información detallada de un contenedor**

```shell
docker inspect <id_contenedor>
```

**Muestra estadísticas de uso de recursos (CPU, RAM, etc.)**

```shell
docker stats
```

---

### Interacción con contenedores

**Abre una terminal dentro del contenedor**

```shell
docker exec -it <id_contenedor> /bin/bash
```

**Ejecuta un comando dentro del contenedor**

```shell
docker exec -it <id_contenedor> <comando>
```

---

### Limpieza

**Elimina imágenes no utilizadas**

```shell
docker image prune
```

**Elimina contenedores, imágenes, volúmenes y redes no usadas**

```shell
docker system prune
```

**Elimina todos los recursos no utilizados, incluyendo imágenes no asociadas**

```shell
docker system prune --all
```

---

## Docker Compose

**Construye e inicia los servicios definidos en compose.yml**

```shell
docker compose up
```

**Inicia los servicios en segundo plano**

```shell
docker compose up -d
```

**Detiene y elimina los contenedores, redes y volúmenes definidos**

```shell
docker compose down
```

**Construye o reconstruye las imágenes definidas**

```shell
docker compose build
```

**Muestra los registros de todos los servicios**

```shell
docker compose logs
```

**Lista los servicios en ejecución**

```shell
docker compose ps
```

**Detiene los contenedores sin eliminarlos**

```shell
docker compose stop
```

**Reinicia los servicios**

```shell
docker compose restart
```

---

## Docker Swarm

**Inicializa un nuevo clúster Swarm en el nodo actual**

```shell
docker swarm init
```

**Hace que el nodo abandone el Swarm (forzadamente)**

```shell
docker swarm leave --force
```

**Despliega una aplicación en modo Swarm usando un archivo Compose**

```shell
docker stack deploy -c <archivo>.yml <nombre_stack>
```

**Lista los servicios activos en el Swarm**

```shell
docker service ls
```

**Muestra los contenedores (tareas) del stack desplegado**

```shell
docker stack ps <nombre_stack>
```

**Muestra información general del sistema, incluyendo estado del Swarm**

```shell
docker info
```

---

## Ejemplo de uso práctico

**Eliminar contenedores e imágenes no usados**

```shell
docker system prune --all
```

**Desplegar stack en modo swarm**

```shell
docker stack deploy -c swarm.yml billing
```

**Revisar servicios activos**

```shell
docker service ls
```

---

