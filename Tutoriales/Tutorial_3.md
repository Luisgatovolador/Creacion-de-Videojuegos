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



https://github.com/user-attachments/assets/bd2485a5-d0a2-4b6a-a895-fd4ff19eafe9


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
<img width="1919" height="1023" alt="image" src="https://github.com/user-attachments/assets/791f29f6-2119-40d6-8809-bc23d7302924" />

### 3.2.2. ¿Cómo restablecer la posición del Background?  
<img width="1919" height="1018" alt="image" src="https://github.com/user-attachments/assets/708c6aaf-dc77-454b-bc35-e77e005269e3" />

### 3.2.3. ¿Cómo corregir la repetición del fondo con colisionador? 
<img width="1919" height="1021" alt="image" src="https://github.com/user-attachments/assets/450a8ebc-765d-42bb-abcf-e4e89ce52fbc" />

### 3.2.4. ¿Cómo agregar un nuevo desencadenador de fin del juego?
<img width="1919" height="1015" alt="image" src="https://github.com/user-attachments/assets/9a11135a-b972-4286-8e75-839527bddc45" />

### 3.2.5. ¿Cómo detener MoveLeft cuando ocurre un gameOver?  
<img width="1919" height="1019" alt="image" src="https://github.com/user-attachments/assets/dcd15a96-9b6d-447c-b541-5add8b9be66e" />

### 3.2.6. ¿Cómo detener la generación de obstáculos durante el gameOver?
<img width="1919" height="1019" alt="image" src="https://github.com/user-attachments/assets/adcdbef8-0eb8-4b47-b7e6-0115d1a82763" />

### 3.2.7. ¿Cómo destruir los obstáculos que sobrepasen los límites?  
<img width="1919" height="1021" alt="image" src="https://github.com/user-attachments/assets/f69fbe6d-2785-42a6-adad-c85c8c37beba" />


---

## Lección 3.3: No te quedes ahí sin hacer nada

### 3.3.1. ¿Cómo explorar las animaciones del jugador? 
<img width="1919" height="1019" alt="image" src="https://github.com/user-attachments/assets/be0e0b20-dbe1-4c6a-b0a0-b4faebfbbba2" />

### 3.3.2. ¿Cómo hacer que el jugador comience corriendo?  
<img width="1919" height="1020" alt="image" src="https://github.com/user-attachments/assets/f8a0cdbf-6118-4438-9b84-4b67e29ca98d" />

### 3.3.3. ¿Cómo configurar una animación de salto? 
<img width="1919" height="1016" alt="image" src="https://github.com/user-attachments/assets/40381772-232f-411c-8ea1-9c6f45ac676e" />

### 3.3.4. ¿Cómo ajustar la animación de salto? 
<img width="1919" height="1016" alt="Captura de pantalla 2025-10-19 001110" src="https://github.com/user-attachments/assets/e6bfd3db-c570-4e0f-904d-325ffbecd251" />

### 3.3.5. ¿Cómo configurar una animación de caída? 
<img width="1919" height="1022" alt="image" src="https://github.com/user-attachments/assets/ca31200f-1408-4192-808b-be81b903a0ec" />

### 3.3.6. ¿Cómo evitar que el jugador salte mientras está inconsciente?  
<img width="1919" height="1025" alt="image" src="https://github.com/user-attachments/assets/ffcb7453-64d9-4001-9262-a35e394900d0" />

---

## Lección 3.4: Efectos de sonido y partículas

### 3.4.1. ¿Cómo personalizar una partícula de explosión?
<img width="1919" height="1014" alt="image" src="https://github.com/user-attachments/assets/4a4ba508-e779-4f3f-b936-ba3ddfbe2571" />

### 3.4.2. ¿Cómo reproducir la partícula al momento de la colisión? 
<img width="1919" height="1023" alt="image" src="https://github.com/user-attachments/assets/a9a66473-603e-462b-951a-14440da2ca1d" />

### 3.4.3. ¿Cómo agregar una partícula de salpicadura de polvo? 
<img width="1919" height="1015" alt="image" src="https://github.com/user-attachments/assets/3fe90f38-2eaa-4608-a916-2429283035ad" />

### 3.4.4. ¿Cómo agregar música al objeto de cámara?  
<img width="1919" height="1015" alt="image" src="https://github.com/user-attachments/assets/2f936eff-1121-4c4b-8f83-5e7d31282cb1" />

### 3.4.5. ¿Cómo declarar variables para Clips de audio?  
<img width="1919" height="1013" alt="image" src="https://github.com/user-attachments/assets/18d498a4-e83b-43f4-a05a-8f2bbf1caa1a" />

### 3.4.6. ¿Cómo reproducir clips de audio al saltar y al chocar?
<img width="1919" height="1023" alt="image" src="https://github.com/user-attachments/assets/766702e8-449b-43a6-8dd5-db408aaef49e" />

