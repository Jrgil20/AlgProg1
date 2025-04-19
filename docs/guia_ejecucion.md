# Guía de Instalación y Ejecución del Autómata Celular Alive

## Requisitos Previos

Para ejecutar el Autómata Celular Alive (Juego de la Vida de Conway) necesitarás:

1. **Sistema Operativo Compatible**: Windows, Linux con Wine, o macOS con Wine/CrossOver.
2. **Free Pascal Compiler (FPC)** o **Lazarus IDE** instalados si deseas compilar el código fuente.

## Opciones para Ejecutar el Programa

### 1. Ejecutar el Archivo Compilado Directamente

La forma más sencilla de ejecutar el programa es utilizando el archivo ejecutable `.exe` ya compilado:

1. Navega a la carpeta `/Proyecto/` del repositorio.
2. Busca el archivo `AC_aliveV2.exe`.
3. Haz doble clic en el archivo ejecutable para iniciar el programa.

En sistemas Linux o macOS:
```bash
wine /ruta/a/AlgProg1/Proyecto/AC_aliveV2.exe
```

### 2. Compilar y Ejecutar desde el Código Fuente

Si deseas compilar el programa desde el código fuente:

1. **Instala Free Pascal Compiler (FPC)**:
   - **Windows**: Descarga e instala desde [freepascal.org](https://www.freepascal.org/)
   - **Linux**: `sudo apt-get install fpc` en distribuciones basadas en Debian
   - **macOS**: Instala vía Homebrew: `brew install fpc`

2. **Compila el código**:
   ```bash
   cd /ruta/a/AlgProg1/Proyecto/
   fpc AC_aliveV2.pas
   ```

3. **Ejecuta el programa**:
   - **Windows**: `AC_aliveV2.exe`
   - **Linux/macOS**: `./AC_aliveV2`

## Uso del Programa

Una vez que el programa esté en ejecución, verás la pantalla de presentación. Presiona Enter para continuar al menú principal.

### Navegación por los Menús

El programa utiliza un sistema de menús para navegar entre diferentes opciones:

1. **Menú Principal**:
   - **Play**: Interactuar con el autómata celular
   - **Settings**: Configurar el programa
   - **Exit**: Salir del programa

2. **Submenú Play**:
   - **Info del Caldo**: Ver información sobre el estado actual
   - **Editar Caldo**: Modificar el estado del autómata
   - **Salir**: Volver al menú principal

3. **Submenú Editar Caldo**:
   - **Avanzar Generación**: Avanzar a través de generaciones
   - **Modificar Caldo**: Editar células individuales
   - **Salir**: Volver al submenú Play

### Configuración de Archivos

El programa puede leer configuraciones iniciales desde archivos y guardar estados en archivos:

1. Por defecto, el programa busca archivos en la ruta `C:\Datos\`
2. Los archivos de entrada deben tener el formato adecuado:
   - Primera línea: `filas,columnas`
   - Líneas siguientes: `fila,columna` para cada célula viva

### Consejos para la Ejecución

- Para una experiencia óptima, ejecuta el programa en una ventana de consola con suficiente tamaño para visualizar correctamente la matriz.
- Si utilizas un terminal con soporte para colores, asegúrate de que esté habilitado para visualizar correctamente los colores del programa.
- En Windows, puedes ejecutar el programa en modo de pantalla completa para una mejor visualización.

## Solución de Problemas Comunes

1. **Problema**: Error "File not found" al iniciar el programa
   **Solución**: Crea la carpeta `C:\Datos\` o modifica la configuración de rutas en el programa.

2. **Problema**: El programa se cierra inmediatamente
   **Solución**: Ejecuta el programa desde una consola de comandos para ver los mensajes de error.

3. **Problema**: Los colores no se muestran correctamente
   **Solución**: Asegúrate de ejecutar el programa en una terminal que soporte colores ANSI.

4. **Problema**: La matriz se muestra desalineada
   **Solución**: Reduce el número de columnas a menos de 40 o ajusta la ventana de la consola.