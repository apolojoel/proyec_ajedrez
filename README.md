Proyecto Ajedrez en Java
Descripción
Este proyecto de ajedrez en Java permite leer y visualizar una partida en formato PGN (Portable Game Notation). Utiliza el entorno gráfico Java Swing para mostrar el tablero de ajedrez y permite avanzar y retroceder en la partida. Los movimientos se leen desde un archivo en formato PGN, y el tablero se actualiza en la interfaz gráfica a medida que se avanza o retrocede en el juego.

Estructura del Proyecto
Paquetes
El proyecto está organizado en los siguientes paquetes:

GUI:

Contiene la clase InterfazGrafica, que maneja la visualización del tablero y la interfaz gráfica en Java Swing.
Jugabilidad:

Pieza: Define la representación de una pieza de ajedrez en el tablero, con métodos para el movimiento y características.
Movimiento: Define los movimientos realizados en la partida y cómo interpretar cada movimiento en el contexto del juego.
Tablero: Maneja el estado del tablero, incluyendo la posición de las piezas y las actualizaciones de estado al realizar un movimiento.
Lector:

Contiene la clase LectorPGN, que se encarga de leer el archivo PGN, extraer los movimientos y convertirlos en una lista para ser interpretados y visualizados en el tablero.
Clases
InterfazGrafica:

Clase principal de la interfaz de usuario. Crea una ventana con Java Swing que muestra el tablero de ajedrez y permite al usuario avanzar y retroceder en los movimientos.
Botones para controlar la partida: avanzar, retroceder y reiniciar.
Carga de imágenes de las piezas y actualiza su posición en el tablero según los movimientos.
Pieza:

Clase que representa una pieza de ajedrez, con atributos como tipo de pieza (rey, reina, torre, etc.) y color.
Define métodos básicos de movimiento y restricciones para cada pieza.
Movimiento:

Clase que interpreta y almacena cada movimiento de la partida.
Permite avanzar o retroceder en la lista de movimientos, modificando el estado del tablero.
Tablero:

Clase que mantiene el estado actual del tablero, incluyendo la posición de cada pieza.
Contiene métodos para actualizar el estado del tablero y aplicar movimientos.
Dibuja el tablero en el área correspondiente de la interfaz gráfica.
LectorPGN:

Clase que lee el archivo PGN y convierte el texto en una lista de movimientos.
Ignora los metadatos y se centra en los movimientos de ajedrez en notación algebraica.
Devuelve una lista de movimientos que Movimiento e InterfazGrafica pueden usar para mostrar el juego.
Ejecución del Programa
Abrir el Proyecto en NetBeans:

Clona el repositorio o descarga el proyecto en tu equipo.
Abre NetBeans y selecciona "Abrir Proyecto" para cargar el proyecto en el IDE.
Compilar y Ejecutar:

Asegúrate de que todos los archivos .png necesarios para las piezas estén en la carpeta adecuada.
Compila el proyecto.
Ejecuta InterfazGrafica, la clase que contiene el método main, y observa el tablero inicial en pantalla.
Interacción:

Usa los botones "Avanzar" y "Retroceder" para moverte entre los movimientos del juego.
Para reiniciar el juego, utiliza el botón correspondiente que carga el estado inicial de la partida.
Requisitos Técnicos
Java JDK 8 o superior.
NetBeans (opcional, aunque recomendado para edición y compilación).
Archivo PGN con movimientos de una partida de ajedrez en notación algebraica estándar.
Personalización (Opcional)
Puedes agregar efectos de sonido, animaciones de movimiento de piezas o cambiar el tema visual del tablero ajustando el código en InterfazGrafica y Tablero. Los sonidos pueden implementarse mediante la clase Clip de Java, y para cambiar temas puedes actualizar las imágenes PNG de las piezas.


