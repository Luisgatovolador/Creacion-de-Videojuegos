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
<img width="1919" height="1025" alt="image" src="https://github.com/user-attachments/assets/f8780073-b278-46b0-98f5-efffc5a725cc" />

### 3.1.2. ¿Cómo elegir y configurar un personaje jugador? 
<img width="1919" height="1028" alt="image" src="https://github.com/user-attachments/assets/de384b43-50fc-4cb6-aa8f-31c5658bb19b" />

### 3.1.3. ¿Cómo hacer que el jugador salte al inicio?  
<img width="1919" height="1015" alt="image" src="https://github.com/user-attachments/assets/9547258f-b3ae-4d6b-ac2b-41cdac5f6812" />

### 3.1.4. ¿Cómo hacer que el jugador salte si se presiona la barra espaciadora?  
<img width="1919" height="1018" alt="image" src="https://github.com/user-attachments/assets/1d87aebd-f050-46e3-82c1-8b524ee0a136" />

### 3.1.5. ¿Cómo corregir la fuerza y la gravedad del salto?  
<img width="1919" height="1022" alt="image" src="https://github.com/user-attachments/assets/4d98c8ec-05c6-40be-aee7-9ce89a4a47bf" />

### 3.1.6. ¿Cómo evitar que el jugador realice saltos dobles?  
<img width="1919" height="1027" alt="image" src="https://github.com/user-attachments/assets/51392759-1bb9-4a2a-b7f1-6c86bfca33db" />

### 3.1.7. ¿Cómo crear un obstáculo y moverlo a la izquierda? 
<img width="1917" height="1019" alt="image" src="https://github.com/user-attachments/assets/5e886b44-8ee6-416f-8551-c1840417cb8a" />

### 3.1.8. ¿Cómo crear un Spawn Manager?  
<img width="1919" height="1017" alt="image" src="https://github.com/user-attachments/assets/6b2cdb01-bf52-48e6-95d7-c05521be4f2c" />

### 3.1.9. ¿Cómo generar obstáculos a intervalos?  
<img width="1919" height="1022" alt="image" src="https://github.com/user-attachments/assets/3d00f1f4-ff93-48ff-bda6-75aa7630b586" />

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
