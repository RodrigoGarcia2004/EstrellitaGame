# ⭐ ESTRELLA GAME

## 📖 INTRODUCCIÓN

**Nombre del juego:** Estrella Game  

**Temática:**  
El juego presenta un **cubo** como personaje principal que debe moverse horizontalmente para **recoger estrellas que caen desde la parte superior de la pantalla**. Hay distintos tipos de estrellas y objetos:

- ⭐ Estrella normal: suma puntos.
- 🌟 Superestrella: suma más puntos que la normal.
- ☄️ Estrella mala / meteorito: resta puntos.
- 🟢 Estrella verde (Power-Up): activa un bonus temporal que aumenta el tamaño del cubo.
- ⚠️ Trampa: termina la partida inmediatamente.

**Objetivo:**  
Recolectar la mayor cantidad de estrellas posible antes de que termine el tiempo, evitando trampas y gestionando correctamente los power-ups.

---

# ⚙️ DESARROLLO

## Lógica del juego

El juego utiliza **LibGDX** para gestionar la lógica y el renderizado:

- **Movimiento del cubo:**  
  El cubo se mueve mediante **teclas izquierda/derecha** o **toques en pantalla**, ajustando su posición X.

- **Colisiones:**  
  Cada estrella tiene un `Rectangle` para su posición y tamaño. Se verifica la colisión con el cubo mediante `overlaps()`. Según el tipo de estrella, se suma o resta puntos, se activa un power-up o se termina el juego.

- **Power-ups y temporizadores:**  
  Algunos objetos activan efectos temporales (por ejemplo, agrandar el cubo). Se manejan mediante variables `powerUpActivo` y `powerUpTimer`.

- **Dificultad progresiva:**  
  A medida que el jugador recoge estrellas, aumenta el nivel, incrementando la velocidad de caída y reduciendo el tiempo entre apariciones.

- **Sistema de puntuación:**  
  Se guarda el **HighScore** usando `Preferences` de LibGDX.

- **Audio:**  
  Se reproducen efectos de sonido al recoger estrellas y música de fondo en bucle.

---

## Estructura del juego

### Clases principales:

- **Estrella.java**: clase principal del juego.
- **MainScreen.java**: pantalla de inicio y navegación.
- **GameScreen.java**: lógica principal del juego, manejo de sprites, audio y colisiones.
- **EstrellaCaida (clase interna en GameScreen)**: representa cada estrella que cae.

### Pantallas:

- **Pantalla de juego (`GameScreen`)**: donde se desarrolla toda la acción y mecánica.
- **Pantalla principal / menú (`MainScreen`)**: inicio del juego y reinicio tras Game Over.

### Assets:

- Imágenes: cubo, estrellas, meteoritos.
- Sonidos: música de fondo y efectos al recoger estrellas.
- Los archivos se cargan desde la carpeta `assets`.

---

# 📝 CONCLUSIONES

- La **representación lógica** (rectángulos para colisiones, posiciones X/Y de objetos) permite detectar interacciones sin depender de la representación gráfica exacta.  
- La **representación gráfica** (sprites, texturas) proporciona la visualización, pero se maneja de manera separada de la lógica para facilitar el control y las colisiones.
- LibGDX facilita la separación entre **lógica del juego y renderizado**, lo que permite manejar física, colisiones y temporizadores sin que afecte directamente al dibujo de los objetos en pantalla.
- Aprendizaje clave: la organización del juego en **clases y pantallas** simplifica la escalabilidad, manejo de estados (Running, Paused, Game Over) y reutilización de código para futuros proyectos.

---

# 🚀 EJECUCIÓN

1. Clonar el repositorio:

```
git clone https://github.com/tuusuario/estrella-game.git
```

2. Abrir el proyecto en **IntelliJ IDEA** o **Eclipse**.

3. Ejecutar la clase **DesktopLauncher** para iniciar el juego.

---

# 👨‍💻 AUTOR

**Rodrigo García Heredia**  
Proyecto desarrollado como práctica de programación de videojuegos con LibGDX.
