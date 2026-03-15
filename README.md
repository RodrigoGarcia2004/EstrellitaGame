# ⭐ ESTRELLA GAME

## 📖 DESCRIPCIÓN

**Estrella Game** es un videojuego desarrollado en **Java utilizando el framework LibGDX**.  
El objetivo del juego es controlar un cubo que debe **recoger estrellas que caen desde la parte superior de la pantalla**, evitando trampas y gestionando el tiempo para conseguir la mayor puntuación posible.

El juego incluye distintos tipos de estrellas, power-ups, niveles progresivos y un sistema de puntuación máxima.

---

# 🎮 MECÁNICA DEL JUEGO

El jugador controla un **cubo** que se mueve horizontalmente por la pantalla para recoger estrellas que caen desde arriba.

Durante la partida aparecen diferentes tipos de objetos:

## ⭐ Tipos de objetos

- ⭐ **Estrella normal**  
  Suma 1 punto.

- 🌟 **Superestrella**  
  Suma más puntos que una estrella normal.

- ☄️ **Estrella mala / meteorito**  
  Resta puntos al jugador.

- 🟢 **Estrella verde (Power-Up)**  
  Activa un bonus temporal que aumenta el tamaño del cubo y facilita recoger estrellas.

- ⚠️ **Trampa**  
  Termina la partida inmediatamente.

---

# 📈 SISTEMA DE PROGRESIÓN

El juego aumenta la dificultad progresivamente mediante:

- Incremento de **velocidad de caída de las estrellas**
- Reducción del **tiempo entre apariciones**
- Sistema de **niveles**
- **Modo contrarreloj**

Cada cierto número de estrellas recogidas el jugador sube de nivel, lo que hace que el juego sea más rápido y desafiante.

---

# 🎯 OBJETIVO DEL JUEGO

El objetivo es **recoger la mayor cantidad de estrellas posible antes de que el tiempo termine**, evitando trampas y gestionando correctamente los power-ups.

Además, el juego guarda la **puntuación máxima (HighScore)** del jugador.

---

# 🕹 CONTROLES

## Teclado

| Acción | Control |
|------|------|
| Mover cubo | Flecha izquierda / derecha |
| Pausar juego | ESC |
| Continuar tras Game Over | Tocar pantalla |

## Pantalla táctil

- Tocar la pantalla para mover el cubo a la posición deseada.

---

# ⚙️ TECNOLOGÍAS UTILIZADAS

- **Java**
- **LibGDX**
- Sistema de audio de LibGDX
- Preferencias de LibGDX para guardar puntuaciones
- Sprites y colisiones mediante Rectangles

---

# 📂 ESTRUCTURA DEL PROYECTO

```
core/
 └─ src/com/bdc/drop/io
      ├─ Estrella.java
      ├─ MainScreen.java
      └─ GameScreen.java

assets/
 ├─ imágenes
 ├─ sonidos
 └─ música
```

---

# 🚀 CÓMO EJECUTAR EL PROYECTO

1. Clonar el repositorio

```
git clone https://github.com/tuusuario/estrella-game.git
```

2. Abrir el proyecto en **IntelliJ IDEA** o **Eclipse**.

3. Ejecutar la clase:

```
DesktopLauncher
```

Esto iniciará la versión de escritorio del juego.

---

# 💾 FUNCIONALIDADES IMPLEMENTADAS

- Sistema de **niveles**
- **Aumento progresivo de dificultad**
- **Modo contrarreloj**
- **Power-ups temporales**
- **Sistema de pausa**
- **Game Over**
- **Sistema de HighScore**
- **Efectos de sonido y música de fondo**

---

# 👨‍💻 AUTOR

Proyecto desarrollado como práctica de **programación de videojuegos con LibGDX**.

Autor: **Rodrigo Garcia Heredia**
