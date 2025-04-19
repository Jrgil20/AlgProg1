# ALGProgr1 - Juego de la Vida de Conway

Implementación del Juego de la Vida de Conway como proyecto para la materia de Algoritmo y Programación 1, segundo semestre con Lia en 2022.

![Banner Juego de la Vida](https://conwaylife.com/w/images/b/b6/Fpento.gif)

## Descripción del Repositorio

¡Bienvenido al repositorio de ALGProgr1!

Este repositorio contiene una colección de ejercicios y el proyecto principal de la materia ALGORITMO Y PROGRAMACION 1. La materia se enfoca en brindar las bases para la programación estructurada utilizando el lenguaje Pascal.

## Estructura del Repositorio

- 📁 **docs/** - Documentación del proyecto
  - 📄 [Visión General del Proyecto](docs/proyecto_overview.md) - Descripción conceptual del Juego de la Vida
  - 📄 [Implementación Técnica](docs/implementacion_tecnica.md) - Detalles técnicos de la implementación
  - 📄 [Guía de Ejecución](docs/guia_ejecucion.md) - Instrucciones para ejecutar el proyecto
  - 📄 [Proyecto-ACA2022.pdf](docs/Proyecto-ACA2022.pdf) - PDF original del proyecto asignado

- 📁 **ejercicios/** - Ejercicios prácticos de programación en Pascal
  - Múltiples ejercicios para practicar los conceptos de programación estructurada

- 📁 **Proyecto/** - Código fuente del Juego de la Vida
  - 📄 [AC_aliveV2.pas](Proyecto/AC_aliveV2.pas) - Código fuente en Pascal
  - 📄 [AC_aliveV2.exe](Proyecto/AC_aliveV2.exe) - Ejecutable compilado

## Cómo Ejecutar el Juego de la Vida

### Windows
1. Navega a la carpeta `/Proyecto/`
2. Haz doble clic en `AC_aliveV2.exe`

### Linux/macOS
1. Instala Wine: `sudo apt install wine` (Ubuntu/Debian) o `brew install --cask wine-stable` (macOS)
2. Ejecuta: `wine /ruta/a/AlgProg1/Proyecto/AC_aliveV2.exe`

### Compilación desde el Código Fuente
```bash
cd /ruta/a/AlgProg1/Proyecto/
fpc AC_aliveV2.pas
# En Windows:
AC_aliveV2.exe
# En Linux/macOS:
./AC_aliveV2
```

Para más detalles sobre la ejecución y configuración, consulta la [Guía de Ejecución](docs/guia_ejecucion.md).

## Sobre el Juego de la Vida

El Juego de la Vida es un autómata celular creado por el matemático John Horton Conway en 1970. Es un juego de cero jugadores, lo que significa que su evolución está determinada por el estado inicial y no necesita ninguna entrada humana mientras se ejecuta.

El "juego" consiste en una cuadrícula de células que evolucionan según reglas simples:

1. Una célula viva con 2 o 3 vecinos vivos sobrevive.
2. Una célula viva con menos de 2 o más de 3 vecinos vivos muere.
3. Una célula muerta con exactamente 3 vecinos vivos se convierte en una célula viva.

Para más detalles sobre el concepto y la implementación, consulta la [Visión General del Proyecto](docs/proyecto_overview.md).

## Contribuciones

¡Las contribuciones son bienvenidas! Si deseas mejorar el código o la documentación, no dudes en crear un pull request.

## Licencia

Este proyecto está licenciado bajo la [Licencia MIT](LICENSE).
