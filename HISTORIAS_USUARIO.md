# Historias de Usuario - Proyecto ROAD FIGHTER Z

Documento derivado de los requisitos funcionales y no funcionales del videojuego ROAD-ROAD-FIGHTER, inspirado en ROAD FIGHTER (Konami, 1984). Cada historia sigue el formato:

> **Como** [rol], **quiero** [acción/funcionalidad], **para** [beneficio/valor]

Incluye criterios de aceptación para poder gestionar cada historia como una tarea independiente (por ejemplo, en GitHub Projects / Issues).

---

## Tabla de Historias de Usuario

| ID | Título | Rol | Prioridad | Origen (Requisito) | Estado |
|----|--------|-----|-----------|--------------------|--------|
| US-01 | Escenario de carretera | Jugador | Alta | RF1 | Pendiente |
| US-02 | Control del vehículo con teclado | Jugador | Alta | RF2, RF3 | Pendiente |
| US-03 | Evitar obstáculos en la carretera | Jugador | Alta | RF4 | Pendiente |
| US-04 | Gestionar el combustible/gasolina | Jugador | Alta | RF4 | Pendiente |
| US-05 | Sistema de puntuación y progreso | Jugador | Alta | RF5 | Pendiente |
| US-06 | Condiciones de victoria y derrota | Jugador | Alta | RF5, RF6 | Pendiente |
| US-07 | Pantalla de estado del juego | Jugador | Media | RF7 | Pendiente |
| US-08 | Menú de inicio y pausa | Jugador | Media | RF9.4 | Pendiente |
| US-09 | Efectos de sonido y animaciones | Jugador | Media | RF9.4 | Pendiente |
| US-10 | Registro de récords / puntajes altos | Jugador | Media | RF9.5 | Pendiente |
| US-11 | Niveles de dificultad progresiva | Jugador | Baja | RF9.1 | Pendiente |
| US-12 | Vidas, bonificaciones o poderes especiales | Jugador | Baja | RF9.3 | Pendiente |
| US-13 | IA sencilla para enemigos/oponentes | Jugador | Baja | RF9.6 | Pendiente |
| US-14 | Ejecutable independiente (.exe) | Desarrollador / Evaluador | Media | RNF6 | Pendiente |
| US-15 | Documento de diseño y UML | Docente / Evaluador | Media | RNF9.2 | Pendiente |
| US-16 | Presentación del proyecto | Equipo | Media | RNF9.4 | Pendiente |

---

## Historias de Usuario Detalladas

---

### US-01 — Escenario de carretera

**Como** jugador,  
**quiero** ver una carretera por la que conducir,  
**para** tener un entorno donde desarrollar la partida.

**Criterios de aceptación:**
1. El sistema muestra una pantalla o escenario de juego que representa una carretera.
2. La carretera es el escenario principal donde ocurre la acción del juego.
3. El escenario se renderiza correctamente al iniciar el juego.

**Origen:** RF1 — Escenario de juego.

---

### US-02 — Control del vehículo con teclado

**Como** jugador,  
**quiero** controlar el coche mediante el teclado (o ratón/dispositivo apropiado),  
**para** moverme por la carretera y evitar los obstáculos.

**Criterios de aceptación:**
1. El vehículo del jugador responde a las entradas del teclado.
2. El movimiento del coche es fluido y coherente dentro de los límites de la carretera.
3. Existe un personaje/objeto controlable como mecanismo principal de interacción.

**Origen:** RF2 — Interacción con el usuario; RF3 — Personaje controlable.

---

### US-03 — Evitar obstáculos en la carretera

**Como** jugador,  
**quiero** detectar y evitar los coches/obstáculos que aparecen en la carretera,  
**para** no chocar y seguir avanzando en la partida.

**Criterios de aceptación:**
1. Aparecen obstáculos (coches) en la carretera durante el juego.
2. El sistema detecta colisiones entre el jugador y los obstáculos mediante hitboxes.
3. Una colisión con un obstáculo tiene una consecuencia negativa en la partida.

**Origen:** RF4 — Reglas del juego.

---

### US-04 — Gestionar el combustible/gasolina

**Como** jugador,  
**quiero** contar con un indicador de gasolina que se agote con el tiempo,  
**para** llegar a la meta antes de quedarme sin combustible.

**Criterios de aceptación:**
1. El vehículo dispone de un nivel de combustible que disminuye durante la partida.
2. Quedarse sin gasolina antes de alcanzar la meta provoca el fin de la partida.
3. El jugador puede ver cuánto combustible le queda en la interfaz.

**Origen:** RF4 — Reglas del juego.

---

### US-05 — Sistema de puntuación y progreso

**Como** jugador,  
**quiero** acumular puntos a medida que avanzo en la carretera,  
**para** saber cuánto he progresado y competir por la mejor puntuación.

**Criterios de aceptación:**
1. El sistema lleva una puntuación basada en el progreso del jugador.
2. La puntuación aumenta conforme el jugador avanza por la carretera.
3. Existe un objetivo de progreso (alcanzar la meta).

**Origen:** RF5 — Sistema de puntuación y progreso.

---

### US-06 — Condiciones de victoria y derrota

**Como** jugador,  
**quiero** saber cuándo gano, pierdo o puedo reiniciar la partida,  
**para** tener claridad sobre el resultado de mi juego y empezar de nuevo si deseo.

**Criterios de aceptación:**
1. Existe una condición clara de victoria (alcanzar la meta).
2. Existen condiciones claras de derrota (colisión o quedarse sin gasolina).
3. El jugador puede reiniciar una nueva partida tras finalizar la anterior.

**Origen:** RF5 — Condiciones de victoria; RF6 — Condiciones de finalización de partida.

---

### US-07 — Pantalla de estado del juego

**Como** jugador,  
**quiero** ver una interfaz que muestre mi puntuación, gasolina y estado actual,  
**para** comprender en tiempo real cómo va mi partida.

**Criterios de aceptación:**
1. Existe una interfaz que muestra el estado actual del juego.
2. La interfaz indica al menos la puntuación y el nivel de combustible.
3. La información es clara y legible durante la partida.

**Origen:** RF7 — Interfaz de estado del juego.

---

### US-08 — Menú de inicio y pausa

**Como** jugador,  
**quiero** contar con menús de inicio y pausa,  
**para** iniciar la partida cuando desee y detenerla temporalmente si lo necesito.

**Criterios de aceptación:**
1. Existe un menú de inicio para comenzar el juego.
2. Existe una pantalla de pausa durante la partida.
3. Los menús tienen estilo retro acorde al juego arcade.

**Origen:** RF9.4 — Menús, pantallas de pausa.

---

### US-09 — Efectos de sonido y animaciones

**Como** jugador,  
**quiero** escuchar efectos de sonido y ver animaciones al jugar,  
**para** tener una experiencia más inmersiva y retro.

**Criterios de aceptación:**
1. El juego reproduce efectos de sonido (formato .wav/.ogg) durante la partida.
2. Existen animaciones simples para el movimiento y eventos del juego.
3. Los recursos de audio y gráficos respetan las licencias y atribuciones correspondientes.

**Origen:** RF9.4 — Efectos de sonido o animaciones; RNF5 — Recursos gráficos y de audio.

---

### US-10 — Registro de récords / puntajes altos

**Como** jugador,  
**quiero** que se guarden mis mejores puntuaciones localmente,  
**para** poder superarlas en futuras partidas.

**Criterios de aceptación:**
1. El sistema guarda los puntajes altos en un archivo local (JSON).
2. Los récords persisten entre sesiones de juego.
3. Se puede consultar el registro de récords desde el menú o pantalla correspondiente.

**Origen:** RF9.5 — Registro de récords o persistencia de puntuaciones.

---

### US-11 — Niveles de dificultad progresiva

**Como** jugador,  
**quiero** que el juego se vuelva más difícil a medida que avanzo,  
**para** mantener el reto y la entretenimiento a lo largo de la partida.

**Criterios de aceptación:**
1. Existen niveles de dificultad que aumentan progresivamente.
2. La dificultad afecta a elementos como velocidad, frecuencia de obstáculos o consumo de gasolina.
3. El progreso de dificultad es visible y justo para el jugador.

**Origen:** RF9.1 — Niveles de dificultad progresiva.

---

### US-12 — Vidas, bonificaciones o poderes especiales

**Como** jugador,  
**quiero** disponer de vidas, bonificaciones o poderes especiales,  
**para** tener más oportunidades y opciones estratégicas durante el juego.

**Criterios de aceptación:**
1. El jugador dispone de un sistema de vidas o energía.
2. Existen bonificaciones o poderes especiales que pueden obtenerse.
3. Estas funcionalidades están completamente implementadas y funcionando.

**Origen:** RF9.3 — Sistema de vidas, energía, bonificaciones o poderes especiales.

---

### US-13 — IA sencilla para enemigos/oponentes

**Como** jugador,  
**quiero** que los coches enemigos tengan un movimiento controlado por IA sencilla,  
**para** enfrentar oponentes que se comporten de forma autónoma en la carretera.

**Criterios de aceptación:**
1. Los enemigos u oponentes se mueven por la carretera sin intervención del jugador.
2. El movimiento de los enemigos implementa una inteligencia artificial sencilla.
3. Existen distintos tipos de enemigos con comportamientos diferentes (polimorfismo).

**Origen:** RF9.6 — Inteligencia artificial sencilla para enemigos u oponentes.

---

### US-14 — Ejecutable independiente (.exe)

**Como** desarrollador o evaluador,  
**quiero** poder compilar el proyecto en un ejecutable independiente (.exe),  
**para** demostrar el juego en vivo sin necesidad de instalar dependencias.

**Criterios de aceptación:**
1. El proyecto se compila a un ejecutable independiente usando PyInstaller.
2. El ejecutable funciona correctamente en el entorno de demostración.
3. Todas las dependencias están incluidas o documentadas para el ejecutable.

**Origen:** RNF6 — Distribución (PyInstaller .exe).

---

### US-15 — Documento de diseño y UML

**Como** docente o evaluador,  
**quiero** revisar un documento de diseño con diagrama UML, clases principales y conceptos POO,  
**para** evaluar la calidad del diseño orientado a objetos del proyecto.

**Criterios de aceptación:**
1. Existe un documento de diseño breve con descripción y reglas del juego.
2. Incluye un diagrama UML con clases principales, atributos y métodos.
3. Justifica las relaciones entre clases y los conceptos POO utilizados (encapsulación, herencia, polimorfismo, abstracción).

**Origen:** RNF9.2 — Documento de diseño; RNF7 — Aplicación de POO.

---

### US-16 — Presentación del proyecto

**Como** miembro del equipo,  
**quiero** exponer el funcionamiento, arquitectura y decisiones técnicas del juego,  
**para** presentar el proyecto final y demostrar lo aprendido en la asignatura.

**Criterios de aceptación:**
1. El equipo prepara una exposición del funcionamiento del videojuego.
2. Se explica la arquitectura y las decisiones de programación tomadas.
3. Todos los integrantes participan y pueden explicar las decisiones técnicas.

**Origen:** RNF9.4 — Presentación del proyecto.

---

## Notas para la gestión en GitHub

Cada historia de usuario puede crearse como un **Issue** independiente en el repositorio de GitHub del proyecto "road figther z", y organizarse en un **Project Board (Kanban)** con columnas como:

- **Backlog** (historias pendientes)
- **To Do** (por hacer)
- **In Progress** (en desarrollo)
- **Review** (en revisión/testing)
- **Done** (completado)

Se recomienda etiquetar cada issue con:
- `tipo: funcional` o `tipo: no-funcional`
- `prioridad: alta`, `prioridad: media` o `prioridad: baja`
- `sprint: 1`, `sprint: 2`, etc.

---

*Documento generado a partir de los requisitos definidos en `REQUISITOS.md` y `README.md` del proyecto ROAD-ROAD-FIGHTER.*
