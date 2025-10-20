# Creación de Videojuegos — Tutorial 4  

> **Universidad Tecnológica del Norte de Guanajuato**  
> **Carrera:** Ingeniería en Desarrollo y Gestión de Software  
> **Materia:** Creación de Videojuegos  
> **Profesor:** Gabriel Barrón Rodríguez  
> **Autor:** Rodríguez López Luis Oswaldo  
> **Grupo:** GIDS5103  

---

## Índice  

- [Video Funcionamiento](#video-funcionamiento)  
- [Lección 5.1: ¿Cómo destruir con un clic?](#lección-51-cómo-destruir-con-un-clic)  
  - [5.1.1. ¿Cómo crear un proyecto y cambiar la vista a 2D?](#511-cómo-crear-un-proyecto-y-cambiar-la-vista-a-2d)  
  - [5.1.2. ¿Cómo crear objetivos buenos y malos?](#512-cómo-crear-objetivos-buenos-y-malos)  
  - [5.1.3. ¿Cómo arrojar los objetos al aire de forma aleatoria?](#513-cómo-arrojar-los-objetos-al-aire-de-forma-aleatoria)  
  - [5.1.4. ¿Cómo cambiar el código complicado con nuevos métodos?](#514-cómo-cambiar-el-código-complicado-con-nuevos-métodos)  
  - [5.1.5. ¿Cómo crear una lista de objetos en Game Manager?](#515-cómo-crear-una-lista-de-objetos-en-game-manager)  
  - [5.1.6. ¿Cómo crear una corrutina para generar objetos?](#516-cómo-crear-una-corrutina-para-generar-objetos)  
  - [5.1.7. ¿Cómo destruir objetivos con clics y sensores?](#517-cómo-destruir-objetivos-con-clics-y-sensores)  

- [Lección 5.2: ¿Cómo monitorizar el puntaje?](#lección-52-cómo-monitorizar-el-puntaje)  
  - [5.2.1. ¿Cómo agregar la posición del texto del puntaje en la pantalla?](#521-cómo-agregar-la-posición-del-texto-del-puntaje-en-la-pantalla)  
  - [5.2.2. ¿Cómo editar las propiedades de Score Text?](#522-cómo-editar-las-propiedades-de-score-text)  
  - [5.2.3. ¿Cómo inicializar la variable y el texto del puntaje?](#523-cómo-inicializar-la-variable-y-el-texto-del-puntaje)  
  - [5.2.4. ¿Cómo crear un nuevo método UpdateScore?](#524-cómo-crear-un-nuevo-método-updatescore)  
  - [5.2.5. ¿Cómo agregar puntos cuando se destruyen los objetivos?](#525-cómo-agregar-puntos-cuando-se-destruyen-los-objetivos)  
  - [5.2.6. ¿Cómo agregar un valor de puntos a cada objetivo?](#526-cómo-agregar-un-valor-de-puntos-a-cada-objetivo)  
  - [5.2.7. ¿Cómo agregar una partícula de explosión?](#527-cómo-agregar-una-partícula-de-explosión)  

- [Lección 5.3: Game Over](#lección-53-game-over)  
  - [5.3.1. ¿Cómo crear un objeto de texto de Game Over?](#531-cómo-crear-un-objeto-de-texto-de-game-over)  
  - [5.3.2. ¿Cómo hacer que aparezca el texto de Game Over?](#532-cómo-hacer-que-aparezca-el-texto-de-game-over)  
  - [5.3.3. ¿Cómo crear la función GameOver?](#533-cómo-crear-la-función-gameover)  
  - [5.3.4. ¿Cómo detener la generación de obstáculos y el puntaje durante un GameOver?](#534-cómo-detener-la-generación-de-obstáculos-y-el-puntaje-durante-un-gameover)  
  - [5.3.5. ¿Cómo agregar un botón Reiniciar?](#535-cómo-agregar-un-botón-reiniciar)  
  - [5.3.6. ¿Cómo hacer que funcione el botón de reinicio?](#536-cómo-hacer-que-funcione-el-botón-de-reinicio)  
  - [5.3.7. ¿Cómo mostrar el botón de reinicio durante el fin del juego?](#537-cómo-mostrar-el-botón-de-reinicio-durante-el-fin-del-juego)  

- [Lección 5.4: ¿Cuál es la dificultad?](#lección-54-cuál-es-la-dificultad)  
  - [5.4.1. ¿Cómo crear el texto del título y los botones del menú?](#541-cómo-crear-el-texto-del-título-y-los-botones-del-menú)  
  - [5.4.2. ¿Cómo agregar un Script DifficultyButton?](#542-cómo-agregar-un-script-difficultybutton)  
  - [5.4.3. ¿Cómo llamar SetDifficulty al hacer clic en el botón?](#543-cómo-llamar-setdifficulty-al-hacer-clic-en-el-botón)  
  - [5.4.4. ¿Cómo hacer que tus botones inicien el juego?](#544-cómo-hacer-que-tus-botones-inicien-el-juego)  
  - [5.4.5. ¿Cómo desactivar la pantalla del título al iniciar el juego?](#545-cómo-desactivar-la-pantalla-del-título-al-iniciar-el-juego)  
  - [5.4.6. ¿Cómo utilizar un parámetro para cambiar la dificultad?](#546-cómo-utilizar-un-parámetro-para-cambiar-la-dificultad)  

---

## Video Funcionamiento  

### Abrir para reproducir:  
*(Agrega aquí tu enlace al video cuando esté disponible)*  

---

## Lección 5.1: ¿Cómo destruir con un clic?

### 5.1.1. ¿Cómo crear un proyecto y cambiar la vista a 2D?  
<img width="1919" height="1020" alt="image" src="https://github.com/user-attachments/assets/fbe42daa-550e-4c6b-88cf-15a1dfc4bd77" />

### 5.1.2. ¿Cómo crear objetivos buenos y malos?  
<img width="1919" height="1019" alt="image" src="https://github.com/user-attachments/assets/2ee1918d-800c-4741-89db-9623225d0da4" />

### 5.1.3. ¿Cómo arrojar los objetos al aire de forma aleatoria?  
<img width="1919" height="1019" alt="image" src="https://github.com/user-attachments/assets/bfa71700-8620-483e-b61f-90f850c833fb" />

### 5.1.4. ¿Cómo cambiar el código complicado con nuevos métodos?  
<img width="1919" height="1022" alt="image" src="https://github.com/user-attachments/assets/8eff28b7-8d1a-45c8-b9a0-a43def702ac6" />

### 5.1.5. ¿Cómo crear una lista de objetos en Game Manager?  
### 5.1.6. ¿Cómo crear una corrutina para generar objetos?  
### 5.1.7. ¿Cómo destruir objetivos con clics y sensores?  

---

## Lección 5.2: ¿Cómo monitorizar el puntaje?

### 5.2.1. ¿Cómo agregar la posición del texto del puntaje en la pantalla?  
### 5.2.2. ¿Cómo editar las propiedades de Score Text?  
### 5.2.3. ¿Cómo inicializar la variable y el texto del puntaje?  
### 5.2.4. ¿Cómo crear un nuevo método UpdateScore?  
### 5.2.5. ¿Cómo agregar puntos cuando se destruyen los objetivos?  
### 5.2.6. ¿Cómo agregar un valor de puntos a cada objetivo?  
### 5.2.7. ¿Cómo agregar una partícula de explosión?  

---

## Lección 5.3: Game Over

### 5.3.1. ¿Cómo crear un objeto de texto de Game Over?  
### 5.3.2. ¿Cómo hacer que aparezca el texto de Game Over?  
### 5.3.3. ¿Cómo crear la función GameOver?  
### 5.3.4. ¿Cómo detener la generación de obstáculos y el puntaje durante un GameOver?  
### 5.3.5. ¿Cómo agregar un botón Reiniciar?  
### 5.3.6. ¿Cómo hacer que funcione el botón de reinicio?  
### 5.3.7. ¿Cómo mostrar el botón de reinicio durante el fin del juego?  

---

## Lección 5.4: ¿Cuál es la dificultad?

### 5.4.1. ¿Cómo crear el texto del título y los botones del menú?  
### 5.4.2. ¿Cómo agregar un Script DifficultyButton?  
### 5.4.3. ¿Cómo llamar SetDifficulty al hacer clic en el botón?  
### 5.4.4. ¿Cómo hacer que tus botones inicien el juego?  
### 5.4.5. ¿Cómo desactivar la pantalla del título al iniciar el juego?  
### 5.4.6. ¿Cómo utilizar un parámetro para cambiar la dificultad?  
