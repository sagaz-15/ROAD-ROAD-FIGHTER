# ROAD-ROAD-FIGHTER
Proyecto de programación orientada a objetos referenciado al videojuego ROAD FIGHTER
Conducción por una carretera; evitar obstáculos y conseguir la mayor puntuación posible.

Road Fighter es un videojuego de carreras y la primera entrega de la serie del mismo nombre producido por Konami y lanzado en los arcades en 1984.​ Fue el primer juego de carreras desarrollado por esta compañía. El objetivo es alcanzar la meta sin chocar los coches que aparecen ni quedarse sin gasolina.

# Integrantes
Santiago Machado Viloria


1. Propósito del reto
Como proyecto final de la asignatura, cada equipo deberá diseñar, desarrollar y presentar un videojuego funcional utilizando los principios y conceptos de la programación orientada a objetos estudiados durante el curso. El objetivo no es únicamente construir un juego que se pueda ejecutar, sino demostrar que la POO permite organizar un programa en componentes con responsabilidades claras, facilitar la reutilización del código y permitir que el sistema pueda ampliarse o modificarse sin reescribirlo por completo.
Cada equipo seleccionará una de las opciones propuestas y desarrollará una versión propia, funcional y suficientemente completa del videojuego elegido.

2. Requisitos de desarrollo
2.1. Funcionamiento del videojuego
Una pantalla o escenario de juego.
Interacción con el usuario mediante teclado, ratón u otro dispositivo apropiado.
Un personaje, jugador, objeto controlable o mecanismo principal de interacción, según el juego elegido.
Reglas que determinen las acciones permitidas y la evolución del juego.
Un sistema de puntuación, progreso u objetivos, con condiciones de victoria cuando corresponda.
Condiciones claras para finalizar una partida, perder, ganar o reiniciar, según corresponda.
Una interfaz que permita comprender el estado actual del juego.
La implementación podrá utilizar bibliotecas gráficas apropiadas para Python, como Pygame, u otra herramienta que se ajuste a la POO.
2.2. Aplicación de la programación orientada a objetos
Clases y objetos. Identificar las entidades principales del juego y representarlas mediante clases. Por ejemplo, un videojuego de fútbol podría incluir Jugador, Balón, Equipo y Partido.
Atributos y métodos. Cada clase deberá contener los datos y comportamientos que correspondan a su responsabilidad.
Encapsulación. Explicar cómo se organiza y controla el acceso al estado de los objetos, procurando evitar modificaciones inconsistentes y manteniendo las reglas del juego.
Herencia. Cuando exista una relación conceptual apropiada, utilizar clases base y especializaciones. No se debe utilizar herencia artificialmente solo para cumplir un requisito.
Polimorfismo y abstracción. Cuando el diseño lo justifique, identificar comportamientos comunes que admitan implementaciones diferentes, por ejemplo, distintos tipos de enemigos con métodos propios de movimiento o ataque.
No se evaluará la cantidad de clases creada, sino la calidad del diseño, la coherencia de las relaciones y la justificación de las decisiones tomadas.

3. Funcionalidades adicionales
Se valorarán mejoras incorporadas más allá de los requisitos mínimos. Algunas posibilidades son:
Niveles de dificultad progresiva.
Nuevos personajes, enemigos, obstáculos o tipos de objetos.
Sistema de vidas, energía, bonificaciones o poderes especiales.
Menús, pausas, efectos de sonido o animaciones.
Registro de récords o persistencia de puntuaciones.
Inteligencia artificial sencilla para controlar enemigos u oponentes.
Nuevos modos de juego.
Diseño gráfico y experiencia de usuario mejorados.
Otras funcionalidades originales, pertinentes y correctamente implementadas.
Las funcionalidades adicionales deberán estar terminadas y demostrarse durante la presentación. Una característica anunciada, pero que no funciona, no se considerará implementada.

4. Entregables
Código fuente. Todos los archivos necesarios para ejecutar el videojuego, organizados de manera comprensible.
Instrucciones de ejecución. Un archivo README o documento breve que explique cómo instalar las dependencias y ejecutar el programa.
Documento de diseño. Informe breve con descripción y reglas del juego, diagrama UML, clases principales, atributos y métodos, justificación de relaciones, conceptos POO utilizados, funcionalidades adicionales y dificultades relevantes.
Videojuego ejecutable. Proyecto preparado para una demostración en vivo.
Presentación del proyecto. Exposición del funcionamiento, arquitectura y decisiones de programación.

5. Recomendaciones 
Seleccionar un alcance realista y desarrollar primero una versión funcional antes de incorporar mejoras.
Utilizar recursos gráficos y sonoros respetando las licencias y atribuciones correspondientes.
Organizar el código y verificar que pueda ejecutarse siguiendo las instrucciones entregadas.
Informar qué herramientas, bibliotecas y recursos externos se utilizaron.
Todos los integrantes deben participar en el desarrollo y estar preparados para explicar las decisiones técnicas.


# Stack tecnologico

| Capa / Área | Tecnología Selección | Rol Principal |
| --- | --- | --- |
| **Lenguaje** | **Python 3.10+** | Base del código; sintaxis limpia para lógica de juego y estados. |
| **Motor de Juego** | **Pygame-CE** | Manejo de ventana, renderizado de sprites, bucle principal y audio. |
| **Física y Colisiones** | `pygame.Rect` + `Vector2` | Movimiento vectorial, aceleración y detección de choque por hitboxes. |
| **Interfaz y Datos** | `pygame-menu` + `JSON` | Menús retro de inicio/pausa y guardado local de puntajes altos. |
| **Assets (Arte y Audio)** | **Aseprite** + **bfxr** (`.wav`/`.ogg`) | Creación de sprites pixel art 8-bit y efectos de sonido arcade. |
| **Distribución** | **PyInstaller** | Compilación del proyecto a un ejecutable independiente (`.exe`). |
