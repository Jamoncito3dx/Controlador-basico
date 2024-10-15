# Unity Character Controller with Jump

Este proyecto implementa un **Character Controller** básico en Unity con la funcionalidad de movimiento y salto. Está diseñado para ser fácil de usar y modificar para proyectos en Unity que requieran control de un jugador en 3D.

## Características

- Movimiento en los ejes X y Z usando las teclas de entrada predeterminadas (`W`, `A`, `S`, `D`).
- Salto con la barra espaciadora (`Space`).
- Detecta si el personaje está en el suelo utilizando una esfera de detección (`groundCheck`).
- Aplica gravedad al personaje para simular física realista.
- Todo el movimiento se maneja a través del componente `CharacterController` de Unity.

## Requisitos

- Unity 2020.3 o superior.
- El GameObject que actuará como jugador debe tener el componente **CharacterController** añadido.
- Es necesario tener un objeto hijo en el jugador que actúe como `groundCheck`, y configurarlo en el inspector.

## Instalación y Uso

1. **Añadir el Script:**
   - Crea un nuevo script llamado `PlayerController` en la carpeta `Scripts` de tu proyecto de Unity.
   - Copia y pega el código del controlador en el script.

2. **Configurar el GameObject:**
   - Crea un GameObject en Unity (por ejemplo, un cubo).
   - Añade el componente **CharacterController** al objeto.
   - Añade el script `PlayerController` al objeto.

3. **Crear GroundCheck:**
   - Crea un objeto vacío dentro del GameObject del jugador y nómbralo `GroundCheck`.
   - Posiciona el objeto `GroundCheck` debajo del personaje, justo al nivel del suelo.

4. **Configuración del Inspector:**
   - Asigna el objeto `GroundCheck` al campo correspondiente en el script.
   - Ajusta la variable `GroundMask` con las capas que representen el suelo.

## Personalización

- **Velocidad:** Puedes ajustar la velocidad del jugador modificando la variable `speed` en el inspector.
- **Altura del salto:** Ajusta la altura del salto modificando la variable `jumpHeight`.
- **Gravedad:** La fuerza de gravedad aplicada al jugador puede ajustarse cambiando la variable `gravity`.

## Ejemplo de Uso

Este script es útil para juegos en 3D donde el jugador necesita moverse y saltar de forma sencilla, por ejemplo:
- Plataformas.
- Aventuras en 3D.
- Juegos de exploración.

## Créditos

Desarrollado como un ejemplo básico para el control de personajes en Unity.

