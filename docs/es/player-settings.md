# Ajustes del reproductor y mando a distancia

_Abre el panel de ajustes de HyperWheel Player con un mando, un teclado, un ratón o la pantalla táctil, y descubre qué hace cada sección._

El panel de ajustes se desliza desde la izquierda del reproductor. La reproducción sigue funcionando detrás. Todo en él funciona con un mando de TV, un teclado, un ratón o una pantalla táctil. El panel se muestra en inglés, así que los nombres de sus opciones aparecen aquí tal como los verás.

## Abrir y cerrar el panel

| Cómo | Para abrir | Para cerrar |
| --- | --- | --- |
| Mando de TV | Pulsa **OK** (o **Seleccionar**, o **Menú** si tu mando lo tiene) | Pulsa **Atrás** |
| Teclado | Pulsa **Enter** o **F2**, o **Ctrl+,** (**Comando+,** en un Mac) | Pulsa **Esc**, o **F2** de nuevo |
| Ratón | Mueve el puntero al borde izquierdo un momento, o haz clic en el borde izquierdo | Haz clic fuera del panel o en la flecha de la parte superior |
| Pantalla táctil | Desliza desde el borde izquierdo | Desliza hacia la izquierda |

El panel se cierra solo tras un minuto sin actividad. La próxima vez se abre en la última sección que usaste.

## Moverse por el panel

- **Arriba** y **Abajo** se mueven entre filas. **Izquierda** y **Derecha** cambian entre la lista de secciones y la sección, o cambian un valor como el tema.
- **OK** selecciona la fila marcada.
- **Atrás** sube un paso: de una sección a la lista de secciones y después se cierra.
- En un Android TV o un Fire TV, **Atrás** no hace nada mientras el panel está cerrado. Para salir de la aplicación, mantén pulsado **Atrás** durante tres segundos.

## Secciones

**Settings**

- **Theme:** sistema, claro u oscuro.
- **Fullscreen:** en un ordenador, si el reproductor ocupa toda la pantalla.
- **On-screen debug:** muestra el estado de la conexión y la reproducción sobre el contenido.
- **Launch on boot:** inicia el reproductor cuando arranca el dispositivo.
- **Display over other apps:** en Android 10 y posteriores, si se permite iniciar con el sistema.
- **Set PIN:** protege **Actions** con un PIN de 4 a 8 dígitos.

**Actions**

- **Reload:** reinicia la página del reproductor.
- **Clear cache:** descarga de nuevo todo el contenido.
- **Unlink this screen:** olvida el código de vinculación para que el dispositivo pueda vincularse a otra Pantalla. La Pantalla en HyperWheel se libera al mismo tiempo.
- **Check for updates** e **Install:** consulta más abajo.
- **Quit:** en un ordenador, cierra la aplicación.

**PWA, System y About** muestran información para soporte: la versión del reproductor, si está en línea y conectado, la Pantalla y la organización, el modelo del dispositivo, el sistema y la versión del visor web, la memoria y el almacenamiento, y la versión de la aplicación. **About** indica además si es una compilación de desarrollo, de pruebas (staging) o de producción; se fija al compilar la aplicación y no se puede cambiar desde ella. **Copy diagnostics** copia todo al portapapeles para que lo pegues en un mensaje a soporte.

Para activar las opciones de desarrollador, que añaden la dirección del servidor a **About** y un ajuste **Remote server** que apunta este reproductor a otro servidor de HyperWheel (desvincula la Pantalla, así que la vinculas de nuevo), abre **About** y selecciona la versión de la aplicación siete veces.

## Proteger los ajustes con un PIN

En **Settings**, selecciona **Set PIN** e introduce de 4 a 8 dígitos dos veces. A partir de entonces, al abrir **Actions** se pide el PIN, una vez cada vez que se abre el panel. Cinco intentos erróneos bloquean el PIN durante 30 segundos, y cada bloqueo posterior dura más.

**¿Olvidaste el PIN?** En HyperWheel, abre el menú de acciones de la Pantalla, luego **Enviar comando a la pantalla** y **Restablecer PIN del reproductor**. La Pantalla debe estar en línea. Si está sin conexión, desinstala y vuelve a instalar la aplicación (o borra sus datos), lo que también elimina el PIN.

## Actualizaciones

- **Windows, macOS y Linux (AppImage):** automáticas cuando se inicia la aplicación.
- **Android, Google TV y Fire TV:** abre **Actions**. Un punto junto a **Actions** significa que hay una versión nueva lista. Selecciona **Install** y confirma en el aviso de Android.

## Relacionado

- [Acerca de la aplicación del reproductor](about-the-player-app.md)
- [Conectar un dispositivo](https://docs.hyperwheel.app/es/screens/connect-a-device/)
