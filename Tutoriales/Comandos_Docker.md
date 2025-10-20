# 📘 Lista de Comandos Docker

**Autor:** 1359  
**Materia:** DevOps  
**Tema:** Comandos Docker (Engine, Compose y Swarm)

---

## 📑 Índice

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

## 🐋 Docker Engine

### 🔹 Imágenes
```shell```
# Lista todas las imágenes descargadas en tu sistema
```docker images```

# Descarga una imagen desde Docker Hub
```
docker pull <imagen>
```
# Elimina una imagen del sistema
docker rmi <id_imagen>

# Busca imágenes en Docker Hub
docker search <nombre>



🔹 Contenedores
# Muestra los contenedores en ejecución
docker ps

# Lista todos los contenedores (activos e inactivos)
docker ps -a

# Crea e inicia un contenedor a partir de una imagen
docker run <imagen>

# Inicia un contenedor en segundo plano
docker run -d <imagen>

# Mapea puertos entre el host y el contenedor
docker run -d -p <puerto_host>:<puerto_contenedor> <imagen>

# Crea un contenedor con un nombre específico
docker run --name <nombre_contenedor> <imagen>



🔹 Control de contenedores
# Inicia un contenedor detenido
docker start <id_contenedor>

# Detiene un contenedor en ejecución
docker stop <id_contenedor>

# Reinicia un contenedor
docker restart <id_contenedor>

# Elimina un contenedor detenido
docker rm <id_contenedor>

# Elimina todos los contenedores detenidos
docker container prune

🔹 Logs y monitoreo
# Muestra los logs de un contenedor
docker logs <id_contenedor>

# Muestra los logs en tiempo real
docker logs -f <id_contenedor>

# Muestra información detallada de un contenedor
docker inspect <id_contenedor>

# Muestra estadísticas de uso de recursos (CPU, RAM, etc.)
docker stats

🔹 Interacción con contenedores
# Abre una terminal dentro del contenedor
docker exec -it <id_contenedor> /bin/bash

# Ejecuta un comando dentro del contenedor
docker exec -it <id_contenedor> <comando>

🔹 Limpieza
# Elimina imágenes no utilizadas
docker image prune

# Elimina contenedores, imágenes, volúmenes y redes no usadas
docker system prune

# Elimina todos los recursos no utilizados, incluyendo imágenes no asociadas
docker system prune --all

⚙️ Docker Compose

# Construye e inicia los servicios definidos en compose.yml
docker compose up

# Inicia los servicios en segundo plano
docker compose up -d

# Detiene y elimina los contenedores, redes y volúmenes definidos
docker compose down

# Construye o reconstruye las imágenes definidas
docker compose build

# Muestra los registros de todos los servicios
docker compose logs

# Lista los servicios en ejecución
docker compose ps

# Detiene los contenedores sin eliminarlos
docker compose stop

# Reinicia los servicios
docker compose restart

🌐 Docker Swarm
# Inicializa un nuevo clúster Swarm en el nodo actual
docker swarm init

# Hace que el nodo abandone el Swarm (forzadamente)
docker swarm leave --force

# Despliega una aplicación en modo Swarm usando un archivo Compose
docker stack deploy -c <archivo>.yml <nombre_stack>

# Lista los servicios activos en el Swarm
docker service ls

# Muestra los contenedores (tareas) del stack desplegado
docker stack ps <nombre_stack>

# Muestra información general del sistema, incluyendo estado del Swarm
docker info


🧹 Ejemplo de uso práctico

# Eliminar contenedores e imágenes no usados
docker system prune --all

# Desplegar stack en modo swarm
docker stack deploy -c swarm.yml billing

# Revisar servicios activos
docker service ls


---

¿Quieres que te lo formatee además con emojis o estilos visuales (por ejemplo, 🧱⚙️🐳 en los títulos) para hacerlo más atractivo al entregar? Puedo darte una versión “estética” del `.md` lista para subir a GitHub o entregar al profesor.











