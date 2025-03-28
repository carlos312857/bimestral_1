# bimestral_1

## Librerías

- **`pygame`**: Usada para crear la ventana del juego, gestionar eventos y dibujar gráficos.
- **`randint`**: Permite generar números aleatorios, utilizado para ubicar los planetas aleatoriamente.

## Inicialización

- **`pygame.init()`**: Inicializa todos los módulos necesarios de Pygame.

## Ventana

- **`ANCHURA_VENTANA = 600`** y **`ALTURA_VENTANA = 600`**: Define el tamaño de la ventana del juego.
- **`COLOR_FONDO = (255, 255, 250)`**: Establece el color de fondo (beige claro).

## Cohete

- **Posición inicial**: El cohete empieza en las coordenadas **(210, 300)**.
- **Movimiento**: El cohete se mueve a la **derecha** con la tecla de flecha **derecha** y vuelve a la **izquierda** al soltar la tecla.

## Planetas

- **Posiciones aleatorias**: Los planetas se generan aleatoriamente en la parte superior de la pantalla utilizando **`randint`**.
- **Movimiento**: Los planetas se desplazan hacia abajo a una velocidad de **2 píxeles por fotograma**.

## Puntuación

- **`PUNTOS`**: Aumenta cada vez que un planeta sale de la pantalla.
- **Marcador**: Muestra la puntuación actual en la esquina inferior izquierda de la pantalla.

## Colisiones

- El juego termina si el cohete colisiona con algún planeta.

## Bucle del Juego

- **Eventos de teclado**: Detecta las teclas presionadas, como la flecha derecha para mover el cohete y la tecla **Escape** para salir del juego.
- **Movimiento de planetas**: Los planetas bajan y, al salir de la pantalla, se reposicionan en la parte superior.
- **Dibujo en pantalla**: Se dibujan el cohete, los planetas y el marcador en cada fotograma del juego.

## Cierre del Juego

- El juego termina si el cohete toca un planeta o si se presiona la tecla **Escape**.
