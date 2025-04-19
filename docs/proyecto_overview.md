# Proyecto: Autómata Celular Alive (Juego de la Vida de Conway)

## Descripción del Proyecto

El Juego de la Vida de Conway es un autómata celular desarrollado por el matemático británico John Horton Conway en 1970. Es un juego de cero jugadores, lo que significa que su evolución está determinada por el estado inicial y no necesita ninguna entrada de humanos mientras se ejecuta.

Este proyecto implementa el Juego de la Vida de Conway en Pascal, proporcionando una interfaz para visualizar la evolución del autómata celular.

## Reglas del Juego

El universo del Juego de la Vida es una cuadrícula ortogonal bidimensional de células cuadradas, cada una de las cuales se encuentra en uno de los dos estados posibles, vivo (1) o muerto (0). Cada célula interactúa con sus ocho vecinos, que son las células adyacentes horizontalmente, verticalmente o en diagonal.

En cada paso de tiempo, ocurren las siguientes transiciones:

1. **Supervivencia**: Una célula viva con exactamente 2 o 3 vecinos vivos sobrevive a la siguiente generación.
2. **Muerte**: Una célula viva con menos de 2 vecinos vivos muere por soledad. Una célula viva con más de 3 vecinos vivos muere por sobrepoblación.
3. **Nacimiento**: Una célula muerta con exactamente 3 vecinos vivos se convierte en una célula viva, como por reproducción.

## Características del Programa

- **Interfaz de Menú**: Permite al usuario navegar entre diferentes opciones a través de un sistema de menú.
- **Visualización del Estado**: Muestra el estado actual del autómata celular y la información relacionada.
- **Edición del Estado**: Permite al usuario editar el estado del autómata celular agregando o eliminando células.
- **Progresión de Generaciones**: Permite al usuario avanzar el autómata celular a través de generaciones, ya sea paso a paso o hasta un número específico de generaciones.
- **Configuración**: Permite al usuario configurar varios aspectos del programa, como la entrada/salida de archivos, dimensiones de la matriz, etc.
- **Interacción con Archivos**: Permite guardar y cargar estados del autómata celular desde y hacia archivos.

## Estructura del Programa

El programa está estructurado en varios procedimientos y funciones que se encargan de diferentes aspectos del juego:

1. **Procedimientos Gráficos**: Encargados de la presentación visual del juego.
2. **Procedimientos de Inicialización, Validación e Impresión**: Encargados de inicializar datos, validar entradas y mostrar información.
3. **Procedimientos de Inspección y Transición**: Encargados de evaluar el estado actual del autómata celular y determinar su próximo estado.
4. **Procedimientos de Ajustes y Modificaciones**: Encargados de permitir al usuario modificar diferentes aspectos del juego.

El programa principal integra todos estos procedimientos y funciones para ofrecer una experiencia completa del Juego de la Vida de Conway.

## Implementación en Pascal

El proyecto está implementado en Pascal, un lenguaje de programación estructurado, lo que permite una organización clara del código en procedimientos y funciones. Se utiliza la unidad Crt para el manejo de la interfaz de consola, permitiendo efectos como colores y posicionamiento del cursor.

## Patrones Interesantes

El Juego de la Vida de Conway es conocido por generar patrones interesantes a partir de configuraciones iniciales simples. Algunos de estos patrones incluyen:

- **Osciladores**: Patrones que vuelven a su estado inicial después de un número finito de generaciones.
- **Naves Espaciales**: Patrones que se trasladan a través de la cuadrícula.
- **Matusalenes**: Patrones que evolucionan durante muchas generaciones antes de estabilizarse.
- **Pistolas de Planeadores**: Patrones que producen continuamente naves espaciales.