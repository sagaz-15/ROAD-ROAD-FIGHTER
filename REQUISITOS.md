# Requisitos del Proyecto ROAD-ROAD-FIGHTER

Documento derivado del `README.md` del proyecto. Contiene los requisitos funcionales y no funcionales del videojuego inspirado en ROAD FIGHTER (Konami, 1984), desarrollado como proyecto final de Programación Orientada a Objetos.

---

## 1. Requisitos Funcionales (RF)
Los requisitos funcionales describen qué debe hacer el sistema, es decir, las características y comportamientos del videojuego.

### RF1 - Escenario de juego
El sistema deberá contar con una pantalla o escenario de juego que represente una carretera por la que el jugador conduce.

### RF2 - Interacción con el usuario
El sistema deberá permitir la interacción del usuario mediante teclado, ratón u otro dispositivo de entrada apropiado para controlar al personaje principal.

### RF3 - Personaje controlable
El sistema deberá incluir un personaje, jugador u objeto controlable (coche) como mecanismo principal de interacción.

### RF4 - Reglas del juego
El sistema deberá definir reglas que determinen las acciones permitidas y la evolución del juego, incluyendo:
- Evitar chocar contra los coches/obstáculos que aparecen en la carretera.
- No quedarse sin gasolina antes de alcanzar la meta.

### RF5 - Sistema de puntuación y progreso
El sistema deberá incluir un sistema de puntuación, progreso u objetivos, con condiciones de victoria cuando correspondan (alcanzar la meta).

### RF6 - Condiciones de finalización de partida
El sistema deberá definir condiciones claras para finalizar una partida:
- Perder (colisión o quedarse sin gasolina).
- Ganar (alcanzar la meta).
- Reiniciar una nueva partida.

### RF7 - Interfaz de estado del juego
El sistema deberá contar con una interfaz que permita al jugador comprender el estado actual del juego (puntuación, gasolina, posición, etc.).

### RF8 - Implementación con biblioteca gráfica
La implementación podrá utilizar bibliotecas gráficas apropiadas para Python, como Pygame, u otra herramienta que se ajuste a la programación orientada a objetos.

---

### RF9 - Funcionalidades adicionales (opcionales y valoradas)

Las siguientes funcionalidades no son obligatorias, pero se valorarán positivamente si están terminadas y funcionando durante la presentación:

- **RF9.1** Niveles de dificultad progresiva.
- **RF9.2** Nuevos personajes, enemigos, obstáculos o tipos de objetos.
- **RF9.3** Sistema de vidas, energía, bonificaciones o poderes especiales.
- **RF9.4** Menús, pantallas de pausa, efectos de sonido o animaciones.
- **RF9.5** Registro de récords o persistencia de puntuaciones (guardado local).
- **RF9.6** Inteligencia artificial sencilla para controlar enemigos u oponentes.
- **RF9.7** Nuevos modos de juego.
- **RF9.8** Diseño gráfico y experiencia de usuario mejorados.
- **RF9.9** Otras funcionalidades originales, pertinentes y correctamente implementadas.

> Nota: una característica anunciada que no funcione no se considerará implementada.

---

## 2. Requisitos No Funcionales (RNF)

Los requisitos no funcionales describen cómo debe ser el sistema: restricciones tecnológicas, de diseño, de calidad y de presentación.

### RNF1 - Lenguaje de programación
El código deberá estar desarrollado en **Python 3.10+**, con sintaxis limpia para la lógica de juego y los estados.

### RNF2 - Motor de juego
El sistema deberá utilizar **Pygame-CE** para el manejo de la ventana, renderizado de sprites, bucle principal y audio.

### RNF3 - Física y detección de colisiones
El movimiento deberá ser vectorial (aceleración y desplazamiento) y la detección de choques se basará en hitboxes utilizando `pygame.Rect` y `Vector2`.

### RNF4 - Interfaz y persistencia de datos
Los menús retro de inicio y pausa deberán implementarse con `pygame-menu`, y el guardado local de puntajes altos se hará mediante archivos **JSON**.

### RNF5 - Recursos gráficos y de audio
Los assets (sprites y sonidos) deberán ser creados con herramientas como **Aseprite** (pixel art 8-bit) y **bfxr** (efectos de sonido en formato `.wav` o `.ogg`), respetando las licencias y atribuciones correspondientes.

### RNF6 - Distribución
El proyecto deberá ser compilable a un ejecutable independiente (`.exe`) utilizando **PyInstaller**, preparado para una demostración en vivo.

---

### RNF7 - Aplicación de Programación Orientada a Objetos (POO)

El diseño del código deberá demostrar el uso adecuado de los principios POO:

- **RNF7.1 - Clases y objetos:** Identificar las entidades principales del juego y representarlas mediante clases y objetos con responsabilidades claras.
- **RNF7.2 - Atributos y métodos:** Cada clase deberá contener los datos (atributos) y comportamientos (métodos) que correspondan a su responsabilidad.
- **RNF7.3 - Encapsulación:** Organizar y controlar el acceso al estado de los objetos, evitando modificaciones inconsistentes y manteniendo las reglas del juego.
- **RNF7.4 - Herencia:** Utilizar clases base y especializaciones cuando exista una relación conceptual apropiada (no usar herencia artificialmente solo para cumplir el requisito).
- **RNF7.5 - Polimorfismo y abstracción:** Identificar comportamientos comunes que admitan implementaciones diferentes (por ejemplo, distintos tipos de enemigos con métodos propios de movimiento o ataque).

> No se evaluará la cantidad de clases creada, sino la calidad del diseño, la coherencia de las relaciones y la justificación de las decisiones tomadas.

---

### RNF8 - Calidad y organización del código

- **RNF8.1** El código fuente deberá estar organizado de manera comprensible.
- **RNF8.2** Deberá incluir un archivo `README` o documento breve que explique cómo instalar las dependencias y ejecutar el programa.
- **RNF8.3** Se deberá informar qué herramientas, bibliotecas y recursos externos se utilizaron.
- **RNF8.4** Se recomienda desarrollar primero una versión funcional antes de incorporar mejoras (alcance realista).

---

### RNF9 - Entregables y presentación

- **RNF9.1** Código fuente completo y organizado.
- **RNF9.2** Documento de diseño breve con: descripción y reglas del juego, diagrama UML, clases principales, atributos y métodos, justificación de relaciones, conceptos POO utilizados, funcionalidades adicionales y dificultades relevantes.
- **RNF9.3** Videojuego ejecutable listo para demostración en vivo.
- **RNF9.4** Presentación del proyecto: exposición del funcionamiento, arquitectura y decisiones de programación.
- **RNF9.5** Todos los integrantes deben participar en el desarrollo y estar preparados para explicar las decisiones técnicas.

---

## 3. Matriz de trazabilidad (resumen)

| ID Requisito | Tipo | Descripción breve | Origen |
|--------------|------|-------------------|--------|
| RF1 | Funcional | Escenario de carretera | README §2.1 |
| RF2 | Funcional | Interacción teclado/ratón | README §2.1 |
| RF3 | Funcional | Personaje controlable | README §2.1 |
| RF4 | Funcional | Reglas de juego (evitar obstáculos, gasolina) | README §2.1 |
| RF5 | Funcional | Puntuación y victoria | README §2.1 |
| RF6 | Funcional | Condiciones de fin de partida | README §2.1 |
| RF7 | Funcional | Interfaz de estado | README §2.1 |
| RF8 | Funcional | Biblioteca gráfica (Pygame) | README §2.1 |
| RF9.x | Funcional (adicional) | Mejoras opcionales valoradas | README §3 |
| RNF1 | No funcional | Python 3.10+ | README Stack |
| RNF2 | No funcional | Pygame-CE | README Stack |
| RNF3 | No funcional | Física y colisiones (Rect + Vector2) | README Stack |
| RNF4 | No funcional | pygame-menu + JSON | README Stack |
| RNF5 | No funcional | Assets Aseprite + bfxr | README Stack |
| RNF6 | No funcional | PyInstaller (.exe) | README Stack |
| RNF7.x | No funcional | Principios POO | README §2.2 |
| RNF8.x | No funcional | Calidad y organización | README §4, §5 |
| RNF9.x | No funcional | Entregables y presentación | README §4, §5 |

---

