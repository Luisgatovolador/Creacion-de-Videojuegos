# Creación de Videojuegos — Tutorial 3

> **Universidad Tecnológica del Norte de Guanajuato**  
> **Carrera:** Ingeniería en Desarrollo y Gestión de Software  
> **Materia:** Creación de Videojuegos  
> **Profesor:** Gabriel Barrón Rodríguez  
> **Autor:** Rodríguez López Luis Oswaldo  
> **Grupo:** GIDS5103  

---

## Índice  

- [Video Funcionamiento](#video-funcionamiento)  
- [Lección 3.1: Fuerza de salto](#lección-31-fuerza-de-salto)  
  - [3.1.1. ¿Cómo abrir el prototipo y cambiar el fondo?](#311-cómo-abrir-el-prototipo-y-cambiar-el-fondo)  
  - [3.1.2. ¿Cómo elegir y configurar un personaje jugador?](#312-cómo-elegir-y-configurar-un-personaje-jugador)  
  - [3.1.3. ¿Cómo hacer que el jugador salte al inicio?](#313-cómo-hacer-que-el-jugador-salte-al-inicio)  
  - [3.1.4. ¿Cómo hacer que el jugador salte si se presiona la barra espaciadora?](#314-cómo-hacer-que-el-jugador-salte-si-se-presiona-la-barra-espaciadora)  
  - [3.1.5. ¿Cómo corregir la fuerza y la gravedad del salto?](#315-cómo-corregir-la-fuerza-y-la-gravedad-del-salto)  
  - [3.1.6. ¿Cómo evitar que el jugador realice saltos dobles?](#316-cómo-evitar-que-el-jugador-realice-saltos-dobles)  
  - [3.1.7. ¿Cómo crear un obstáculo y moverlo a la izquierda?](#317-cómo-crear-un-obstáculo-y-moverlo-a-la-izquierda)  
  - [3.1.8. ¿Cómo crear un Spawn Manager?](#318-cómo-crear-un-spawn-manager)  
  - [3.1.9. ¿Cómo generar obstáculos a intervalos?](#319-cómo-generar-obstáculos-a-intervalos)  

- [Lección 3.2: Haz que el mundo pase volando](#lección-32-haz-que-el-mundo-pase-volando)  
  - [3.2.1. ¿Cómo crear un script para repetir el fondo?](#321-cómo-crear-un-script-para-repetir-el-fondo)  
  - [3.2.2. ¿Cómo restablecer la posición del Background?](#322-cómo-restablecer-la-posición-del-background)  
  - [3.2.3. ¿Cómo corregir la repetición del fondo con colisionador?](#323-cómo-corregir-la-repetición-del-fondo-con-colisionador)  
  - [3.2.4. ¿Cómo agregar un nuevo desencadenador de fin del juego?](#324-cómo-agregar-un-nuevo-desencadenador-de-fin-del-juego)  
  - [3.2.5. ¿Cómo detener MoveLeft cuando ocurre un gameOver?](#325-cómo-detener-moveleft-cuando-ocurre-un-gameover)  
  - [3.2.6. ¿Cómo detener la generación de obstáculos durante el gameOver?](#326-cómo-detener-la-generación-de-obstáculos-durante-el-gameover)  
  - [3.2.7. ¿Cómo destruir los obstáculos que sobrepasen los límites?](#327-cómo-destruir-los-obstáculos-que-sobrepasen-los-límites)  

- [Lección 3.3: No te quedes ahí sin hacer nada](#lección-33-no-te-quedes-ahí-sin-hacer-nada)  
  - [3.3.1. ¿Cómo explorar las animaciones del jugador?](#331-cómo-explorar-las-animaciones-del-jugador)  
  - [3.3.2. ¿Cómo hacer que el jugador comience corriendo?](#332-cómo-hacer-que-el-jugador-comience-corriendo)  
  - [3.3.3. ¿Cómo configurar una animación de salto?](#333-cómo-configurar-una-animación-de-salto)  
  - [3.3.4. ¿Cómo ajustar la animación de salto?](#334-cómo-ajustar-la-animación-de-salto)  
  - [3.3.5. ¿Cómo configurar una animación de caída?](#335-cómo-configurar-una-animación-de-caída)  
  - [3.3.6. ¿Cómo evitar que el jugador salte mientras está inconsciente?](#336-cómo-evitar-que-el-jugador-salte-mientras-está-inconsciente)  

- [Lección 3.4: Efectos de sonido y partículas](#lección-34-efectos-de-sonido-y-partículas)  
  - [3.4.1. ¿Cómo personalizar una partícula de explosión?](#341-cómo-personalizar-una-partícula-de-explosión)  
  - [3.4.2. ¿Cómo reproducir la partícula al momento de la colisión?](#342-cómo-reproducir-la-partícula-al-momento-de-la-colisión)  
  - [3.4.3. ¿Cómo agregar una partícula de salpicadura de polvo?](#343-cómo-agregar-una-partícula-de-salpicadura-de-polvo)  
  - [3.4.4. ¿Cómo agregar música al objeto de cámara?](#344-cómo-agregar-música-al-objeto-de-cámara)  
  - [3.4.5. ¿Cómo declarar variables para Clips de audio?](#345-cómo-declarar-variables-para-clips-de-audio)  
  - [3.4.6. ¿Cómo reproducir clips de audio al saltar y al chocar?](#346-cómo-reproducir-clips-de-audio-al-saltar-y-al-chocar)  

---

## Video Funcionamiento

### Abrir para reproducir:  


---

## Lección 3.1: Fuerza de salto

### 3.1.1. ¿Cómo abrir el prototipo y cambiar el fondo?  
### 3.1.2. ¿Cómo elegir y configurar un personaje jugador?  
### 3.1.3. ¿Cómo hacer que el jugador salte al inicio?  
### 3.1.4. ¿Cómo hacer que el jugador salte si se presiona la barra espaciadora?  
### 3.1.5. ¿Cómo corregir la fuerza y la gravedad del salto?  
### 3.1.6. ¿Cómo evitar que el jugador realice saltos dobles?  
### 3.1.7. ¿Cómo crear un obstáculo y moverlo a la izquierda?  
### 3.1.8. ¿Cómo crear un Spawn Manager?  
### 3.1.9. ¿Cómo generar obstáculos a intervalos?  

---

## Lección 3.2: Haz que el mundo pase volando

### 3.2.1. ¿Cómo crear un script para repetir el fondo?  
### 3.2.2. ¿Cómo restablecer la posición del Background?  
### 3.2.3. ¿Cómo corregir la repetición del fondo con colisionador?  
### 3.2.4. ¿Cómo agregar un nuevo desencadenador de fin del juego?  
### 3.2.5. ¿Cómo detener MoveLeft cuando ocurre un gameOver?  
### 3.2.6. ¿Cómo detener la generación de obstáculos durante el gameOver?  
### 3.2.7. ¿Cómo destruir los obstáculos que sobrepasen los límites?  

---

## Lección 3.3: No te quedes ahí sin hacer nada

### 3.3.1. ¿Cómo explorar las animaciones del jugador?  
### 3.3.2. ¿Cómo hacer que el jugador comience corriendo?  
### 3.3.3. ¿Cómo configurar una animación de salto?  
### 3.3.4. ¿Cómo ajustar la animación de salto?  
### 3.3.5. ¿Cómo configurar una animación de caída?  
### 3.3.6. ¿Cómo evitar que el jugador salte mientras está inconsciente?  

---

## Lección 3.4: Efectos de sonido y partículas

### 3.4.1. ¿Cómo personalizar una partícula de explosión?  
### 3.4.2. ¿Cómo reproducir la partícula al momento de la colisión?  
### 3.4.3. ¿Cómo agregar una partícula de salpicadura de polvo?  
### 3.4.4. ¿Cómo agregar música al objeto de cámara?  
### 3.4.5. ¿Cómo declarar variables para Clips de audio?  
### 3.4.6. ¿Cómo reproducir clips de audio al saltar y al chocar?  
