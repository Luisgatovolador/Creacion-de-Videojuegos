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


https://github.com/user-attachments/assets/672d4e9a-c3ea-4fe3-8632-a318529b5c42



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
<img width="1919" height="1026" alt="image" src="https://github.com/user-attachments/assets/b46ee08e-6a9e-4814-925a-c7d181f8a4d0" />

### 5.1.6. ¿Cómo crear una corrutina para generar objetos? 
<img width="1919" height="1023" alt="image" src="https://github.com/user-attachments/assets/417741aa-1f59-42c9-bfcf-5af82657a6b8" />

### 5.1.7. ¿Cómo destruir objetivos con clics y sensores?  
<img width="1919" height="1021" alt="image" src="https://github.com/user-attachments/assets/36b42607-c91a-4e17-9718-70b055ff4bbe" />


---

## Lección 5.2: ¿Cómo monitorizar el puntaje?

### 5.2.1. ¿Cómo agregar la posición del texto del puntaje en la pantalla?  
<img width="1919" height="1019" alt="image" src="https://github.com/user-attachments/assets/e23b135b-ebbb-405a-92cc-26672a9fb7fb" />

### 5.2.2. ¿Cómo editar las propiedades de Score Text?  
<img width="1919" height="1022" alt="image" src="https://github.com/user-attachments/assets/e2dbc627-5b81-4caf-ac5e-6cdd24cbc131" />

### 5.2.3. ¿Cómo inicializar la variable y el texto del puntaje? 
<img width="1919" height="1019" alt="image" src="https://github.com/user-attachments/assets/b104fe81-8c27-401e-bc4f-d5d267ee8203" />

### 5.2.4. ¿Cómo crear un nuevo método UpdateScore?  
<img width="1919" height="1018" alt="image" src="https://github.com/user-attachments/assets/11da1c0f-fd09-42c2-8ae2-2716a264ce73" />

### 5.2.5. ¿Cómo agregar puntos cuando se destruyen los objetivos? 
<img width="1919" height="1015" alt="image" src="https://github.com/user-attachments/assets/fe8bd73c-80f3-4958-b0cd-f2b5a490df92" />

### 5.2.6. ¿Cómo agregar un valor de puntos a cada objetivo? 
<img width="1919" height="1021" alt="image" src="https://github.com/user-attachments/assets/8a30c973-4c36-48bf-b2ea-8c405c75c1c5" />

### 5.2.7. ¿Cómo agregar una partícula de explosión?  
<img width="1919" height="1019" alt="image" src="https://github.com/user-attachments/assets/e9dfde89-c654-4f4c-9580-6fe7ad4625f2" />


---

## Lección 5.3: Game Over

### 5.3.1. ¿Cómo crear un objeto de texto de Game Over?  
<img width="1914" height="1012" alt="image" src="https://github.com/user-attachments/assets/c85092d4-38f8-4175-9f9e-027165ffaa8a" />

### 5.3.2. ¿Cómo hacer que aparezca el texto de Game Over?  
<img width="1919" height="1020" alt="image" src="https://github.com/user-attachments/assets/f3d235a5-dc16-41be-9643-41ac1b366394" />

### 5.3.3. ¿Cómo crear la función GameOver?  
<img width="1919" height="1023" alt="image" src="https://github.com/user-attachments/assets/27fc5116-b588-4170-b190-047fe82051fc" />

### 5.3.4. ¿Cómo detener la generación de obstáculos y el puntaje durante un GameOver?  
<img width="1919" height="1018" alt="image" src="https://github.com/user-attachments/assets/09400f63-7003-48c7-9ca4-b6a15ebb7830" />

<img width="1919" height="1017" alt="image" src="https://github.com/user-attachments/assets/f7f071a1-f6e2-4bc8-a8a8-85aa1c1999f7" />

### 5.3.5. ¿Cómo agregar un botón Reiniciar?  
<img width="1919" height="1012" alt="image" src="https://github.com/user-attachments/assets/32b9bad5-c66b-44f1-8be7-c2eac74d4343" />

### 5.3.6. ¿Cómo hacer que funcione el botón de reinicio?  
<img width="1919" height="1021" alt="image" src="https://github.com/user-attachments/assets/67d8672c-aa5d-4559-938f-410834906bd4" />

### 5.3.7. ¿Cómo mostrar el botón de reinicio durante el fin del juego?  
<img width="1919" height="1021" alt="image" src="https://github.com/user-attachments/assets/f819a64d-3427-4e7c-8ced-14cb3f4591b1" />

<img width="1919" height="1019" alt="image" src="https://github.com/user-attachments/assets/2d4f5bfa-c6bd-4aef-b720-a5df8a67bb26" />


---

## Lección 5.4: ¿Cuál es la dificultad?

### 5.4.1. ¿Cómo crear el texto del título y los botones del menú? 
<img width="1919" height="1014" alt="image" src="https://github.com/user-attachments/assets/c88c9b2f-ff6c-41ea-931a-210062e70147" />

### 5.4.2. ¿Cómo agregar un Script DifficultyButton?  
<img width="1919" height="1022" alt="image" src="https://github.com/user-attachments/assets/c4630957-693c-4490-b27c-be1141713e2e" />

### 5.4.3. ¿Cómo llamar SetDifficulty al hacer clic en el botón?  
<img width="1918" height="1023" alt="image" src="https://github.com/user-attachments/assets/fcfe9a73-e579-4452-b190-2ee314b554ed" />

### 5.4.4. ¿Cómo hacer que tus botones inicien el juego?  
<img width="1919" height="1015" alt="image" src="https://github.com/user-attachments/assets/a56ddbf4-47cb-4b61-a2c9-9b701b0bd974" />
<img width="1919" height="1019" alt="image" src="https://github.com/user-attachments/assets/acc6084d-27e6-4c7f-8169-b8f4b0fe044e" />


### 5.4.5. ¿Cómo desactivar la pantalla del título al iniciar el juego?
<img width="1919" height="1023" alt="image" src="https://github.com/user-attachments/assets/35bfaa1b-f9ef-44c5-87ac-ab08f1c88859" />
<img width="1919" height="1030" alt="image" src="https://github.com/user-attachments/assets/bb83aae9-11be-4f30-83a1-1f17f0c69393" />
<img width="1919" height="1019" alt="image" src="https://github.com/user-attachments/assets/449e229c-09db-42f4-bc89-a77a58778e08" />



### 5.4.6. ¿Cómo utilizar un parámetro para cambiar la dificultad?  
<img width="1919" height="1014" alt="image" src="https://github.com/user-attachments/assets/613bf2a9-80a4-4195-8fb7-7b95245020e7" />

<img width="1919" height="1037" alt="image" src="https://github.com/user-attachments/assets/ef4eb86d-1727-4939-ba3b-52d2b15644b1" />

<img width="1919" height="1021" alt="image" src="https://github.com/user-attachments/assets/d9b5c36a-b166-4cc0-abcb-eec714849284" />

