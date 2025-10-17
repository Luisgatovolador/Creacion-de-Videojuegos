# Creación de Videojuegos — Tutorial 2  

> **Universidad Tecnológica del Norte de Guanajuato**  
> **Carrera:** Ingeniería en Desarrollo y Gestión de Software  
> **Materia:** Creación de Videojuegos  
> **Profesor:** Gabriel Barrón Rodríguez  
> **Autor:** Rodríguez López Luis Oswaldo  
> **Grupo:** GIDS5103  

---

## Índice  
- [Video Funcionamiento](#video-funcionamiento)
- [Lección 2.1: Posición del jugador](#lección-21-posición-del-jugador)
  - [2.1 ¿Cómo crear un proyecto nuevo para el prototipo 2?](#21cómo-crear-un-proyecto-nuevo-para-el-prototipo-2)
  - [2.2 ¿Cómo añadir al jugador, los animales y la comida?](#22cómo-añadir-al-jugador-los-animales-y-la-comida)
  - [2.3 ¿Cómo obtener la entrada horizontal del usuario?](#23cómo-obtener-la-entrada-horizontal-del-usuario)
  - [2.4 ¿Cómo mover al jugador de izquierda a derecha?](#24cómo-mover-al-jugador-de-izquierda-a-derecha)
  - [2.5 ¿Cómo mantener al jugador dentro de los límites?](#25cómo-mantener-al-jugador-dentro-de-los-límites)
  - [2.6 ¿Cómo limpiar el código y las variables?](#26cómo-limpiar-el-código-y-las-variables)
- [Lección 2.2: Comida voladora](#lección-22-comida-voladora)
  - [2.2.1 ¿Cómo hacer que el proyectil vuele hacia adelante?](#221cómo-hacer-que-el-proyectil-vuele-hacia-adelante)
  - [2.2.2 ¿Cómo convertir el proyectil en un Prefab?](#222cómo-convertir-el-proyectil-en-un-prefab)
  - [2.2.3 ¿Cómo probar la pulsación de la barra espaciadora?](#223cómo-probar-la-pulsación-de-la-barra-espaciadora)
  - [2.2.4 ¿Cómo lanzar un proyectil cuando se pulsa la barra espaciadora?](#224cómo-lanzar-un-proyectil-cuando-se-pulsa-la-barra-espaciadora)
  - [2.2.5 ¿Cómo convertir los animales en Prefabs?](#225cómo-convertir-los-animales-en-prefabs)
  - [2.2.6 ¿Cómo destruir los proyectiles fuera de la pantalla?](#226cómo-destruir-los-proyectiles-fuera-de-la-pantalla)
  - [2.2.7 ¿Cómo destruir los animales fuera de la pantalla?](#227cómo-destruir-los-animales-fuera-de-la-pantalla)
- [Lección 2.3: Estampida de animales aleatorios](#lección-23-estampida-de-animales-aleatorios)
  - [2.3.1 Crea un gestor de generación](#231-crea-un-gestor-de-generación)
  - [2.3.2 Genera un animal cuando se pulsa la tecla S](#232-genera-un-animal-cuando-se-pulsa-la-tecla-s)
  - [2.3.3 Generar animales aleatorios desde el arreglo](#233-generar-animales-aleatorios-desde-el-arreglo)
  - [2.3.4 Establece al azar la ubicación de la generación](#234-establece-al-azar-la-ubicación-de-la-generación)
  - [2.3.5 Cambia la perspectiva de la cámara](#235-cambia-la-perspectiva-de-la-cámara)
- [Lección 2.4: Decisiones de colisiones](#lección-24-decisiones-de-colisiones)
  - [2.4.1 Haz un nuevo método para generar animales](#241-haz-un-nuevo-método-para-generar-animales)
  - [2.4.2 Genera animales en intervalos de tiempo](#242-genera-animales-en-intervalos-de-tiempo)
  - [2.4.3 Agrega un componente Collider y Trigger](#243-agrega-un-componente-collider-y-trigger)
  - [2.4.4 Destruye objetos al colisionar](#244-destruye-objetos-al-colisionar)
  - [2.4.5 Desencadena un mensaje de Game Over](#245-desencadena-un-mensaje-de-game-over)

---
## Video Funcionamiento


https://github.com/user-attachments/assets/575415ab-3c81-4926-a0e4-fab88b644480



## Lección 2.1: Posición del jugador  

### 2.1 ¿Cómo crear un proyecto nuevo para el prototipo 2?  
<img width="1919" height="1079" alt="Captura de pantalla 2025-10-17 085700" src="https://github.com/user-attachments/assets/34d93ee4-7be1-4568-b49b-f87ac8abee24" />

---

### 2.2 ¿Cómo añadir al jugador, los animales y la comida?  
<img width="1919" height="1079" alt="Captura de pantalla 2025-10-17 090428" src="https://github.com/user-attachments/assets/314c0e7e-22ca-47ab-8a4b-37c80bb6879f" />

---

### 2.3 ¿Cómo obtener la entrada horizontal del usuario?  
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/0ccbd42c-8636-47a1-af7b-2775b31d6350" />  
<img width="1919" height="1015" alt="image" src="https://github.com/user-attachments/assets/48f1df9b-c413-4772-8a16-ea055736f266" />

---

### 2.4 ¿Cómo mover al jugador de izquierda a derecha?  
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/1ac4ac36-976e-4ad2-9c1c-9800e8ea73c4" />  
<img width="1919" height="1017" alt="image" src="https://github.com/user-attachments/assets/4f615416-f809-422a-9ec3-e7fbc6cc56a2" />

---

### 2.5 ¿Cómo mantener al jugador dentro de los límites?  
<img width="1919" height="1027" alt="image" src="https://github.com/user-attachments/assets/fba68334-92c5-48a8-b2ff-01419f42459b" />  
<img width="1919" height="1019" alt="image" src="https://github.com/user-attachments/assets/3828f14e-64f8-45ab-950e-4a908727abda" />

---

### 2.6 ¿Cómo limpiar el código y las variables?  
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/8cbc5a28-19ad-41c3-811c-84a6c148d377" />

---

## Lección 2.2: Comida voladora  

### 2.2.1 ¿Cómo hacer que el proyectil vuele hacia adelante? 
<img width="1919" height="1078" alt="image" src="https://github.com/user-attachments/assets/a386222e-3a0d-4006-af82-3288ce3035dc" />

### 2.2.2 ¿Cómo convertir el proyectil en un Prefab?  
<img width="1919" height="1024" alt="image" src="https://github.com/user-attachments/assets/e3d95c6f-84ce-4fc3-bb9e-87ed838d311c" />

### 2.2.3 ¿Cómo probar la pulsación de la barra espaciadora?  
<img width="1919" height="1025" alt="image" src="https://github.com/user-attachments/assets/f6f8292a-7467-46dd-b209-ab114fd8d358" />

### 2.2.4 ¿Cómo lanzar un proyectil cuando se pulsa la barra espaciadora?  
<img width="1919" height="1017" alt="image" src="https://github.com/user-attachments/assets/5458edb1-6652-4f90-89bf-3528677bb6ef" />


### 2.2.5 ¿Cómo convertir los animales en Prefabs?  
<img width="1919" height="1017" alt="image" src="https://github.com/user-attachments/assets/e0ade697-1387-407d-bfdb-67c85f0b1f9c" />

### 2.2.6 ¿Cómo destruir los proyectiles fuera de la pantalla?  
<img width="1919" height="1015" alt="image" src="https://github.com/user-attachments/assets/5cf95799-fbeb-474c-ad0c-c977a11c18a5" />

### 2.2.7 ¿Cómo destruir los animales fuera de la pantalla?  
<img width="1919" height="1019" alt="image" src="https://github.com/user-attachments/assets/d83ed791-b3fe-4066-9600-5ac565c3c690" />


---

## Lección 2.3: Estampida de animales aleatorios  

### 2.3.1 Crea un gestor de generación  
<img width="1919" height="1024" alt="image" src="https://github.com/user-attachments/assets/9179aadb-13f7-4622-a76a-92a1ac2b2355" />

### 2.3.2 Genera un animal cuando se pulsa la tecla S  
<img width="1919" height="1032" alt="image" src="https://github.com/user-attachments/assets/54465219-a5bd-4445-86ad-28dfd797576d" />

### 2.3.3 Generar animales aleatorios desde el arreglo  
<img width="1919" height="1013" alt="image" src="https://github.com/user-attachments/assets/359696ac-189e-411e-9e52-3c4327877706" />

### 2.3.4 Establece al azar la ubicación de la generación  
<img width="1919" height="1022" alt="image" src="https://github.com/user-attachments/assets/7f0e4f71-68c7-4c79-867f-37c8ea65bd3f" />

### 2.3.5 Cambia la perspectiva de la cámara  
<img width="1919" height="1028" alt="image" src="https://github.com/user-attachments/assets/89a5245c-3517-4f13-b29f-21f7df3a4562" />


---

## Lección 2.4: Decisiones de colisiones  

### 2.4.1 Haz un nuevo método para generar animales  
<img width="1919" height="1023" alt="image" src="https://github.com/user-attachments/assets/7dea4b28-f02f-42e1-8a20-81a065b658c2" />

### 2.4.2 Genera animales en intervalos de tiempo  
<img width="1919" height="1024" alt="image" src="https://github.com/user-attachments/assets/e43a1516-cc08-4b0a-99af-3f21862231eb" />

### 2.4.3 Agrega un componente Collider y Trigger  
<img width="1919" height="1021" alt="image" src="https://github.com/user-attachments/assets/edfb133d-e187-4caf-a83c-8337802bf17b" />

### 2.4.4 Destruye objetos al colisionar  
<img width="1919" height="1022" alt="image" src="https://github.com/user-attachments/assets/6f707726-0419-4a16-a8c0-48a81ecc2aba" />

### 2.4.5 Desencadena un mensaje de «Game Over» 
<img width="1919" height="1018" alt="image" src="https://github.com/user-attachments/assets/998895bf-43cf-4539-bf63-5277bddb3040" />


