# Acerca de la aplicación del reproductor

_Qué es la aplicación HyperWheel Player, qué dispositivos admite y cómo descargarla e instalarla._

La aplicación HyperWheel Player reproduce el contenido de tu Pantalla a pantalla completa en un ordenador, un dispositivo Android o un televisor. Es el mismo reproductor que obtienes al abrir [hypr.onl](https://hypr.onl) en un navegador, dentro de una aplicación que puede iniciarse sola, mantenerse en primer plano y mostrar un panel de ajustes que puedes manejar con un mando de TV.

No necesitas la aplicación para usar HyperWheel. Un navegador sirve para muchas instalaciones. Usa la aplicación cuando el dispositivo deba empezar a reproducir solo después de un corte de luz, cuando no tenga teclado ni ratón, o cuando quieras manejarlo con un mando a distancia.

El panel de ajustes de la aplicación se muestra en inglés. En esta guía, los nombres de sus opciones aparecen tal como los verás.

## Dispositivos compatibles

| Dispositivo | Guía de instalación | Estado |
| --- | --- | --- |
| Windows 10 (1809 o posterior) y Windows 11 | Instalar en Windows | Creada, aún no probada en un PC con Windows |
| macOS 12 o posterior, Intel y Apple Silicon | [Instalar en macOS](https://docs.hyperwheel.app/es/player-app/install-on-macos/) | Probada en un Mac |
| Debian, Ubuntu, Fedora y Raspberry Pi OS | [Instalar en Linux](https://docs.hyperwheel.app/es/player-app/install-on-linux/) | Paquetes probados en contenedores, aún no en equipos reales |
| Teléfonos y tabletas Android | [Instalar en Android](install-on-android.md) | Probada en un emulador |
| Google TV y Android TV | [Instalar en Google TV y Android TV](install-on-android-tv.md) | Probada en un emulador, aún no en un televisor |
| Fire TV (Fire OS 7 o posterior) | Instalar en Fire TV | Creada, aún no probada en un Fire TV |
| ChromeOS | Instalar en ChromeOS | Creada, aún no probada en un Chromebook |

**Por ahora solo se puede descargar la aplicación para Android.** Las aplicaciones para Windows, macOS y Linux aún no se han publicado.

Los dispositivos Android necesitan Android 7 o posterior. Los Fire TV más antiguos (Fire TV Stick de 1.ª y 2.ª generación y cualquier dispositivo con Fire OS 5) no pueden ejecutar la aplicación.

Las guías marcadas como "aún no probadas" solo se publican cuando alguien las ha seguido en el dispositivo. Hasta entonces, considéralas sin probar.

## Descargar la aplicación

Descarga desde la página **Aplicaciones del reproductor** de HyperWheel, que destaca el archivo adecuado para tu dispositivo. En un televisor puedes escribir una dirección corta: **hypr.onl/get**. En un dispositivo Android descarga la aplicación directamente. En cualquier otro, abre la lista de descargas.

Todas las descargas se publican en la [página de versiones de HyperWheel Player](https://github.com/AstrohubPty/HyperWheelPlayers/releases/latest), junto con un archivo `SHA256SUMS.txt`. Para comprobar una descarga, compara su suma de verificación SHA-256 con la que aparece allí.

## Por qué aparece una advertencia de seguridad

La aplicación aún no está firmada con un certificado de desarrollador de Windows ni de Apple, por lo que Windows SmartScreen y macOS Gatekeeper avisan antes de la primera ejecución. Las guías de instalación muestran cómo continuar. La advertencia se debe a la falta del certificado. No significa que el archivo esté dañado. Si tienes dudas, comprueba primero la suma de verificación del archivo.

Android muestra su propio aviso la primera vez que instalas una aplicación que no viene de Play Store.

## Vincular la pantalla

Después de instalar, abre la aplicación. Muestra **Link this screen** con un código QR y un código de dispositivo. Sigue [Conectar un dispositivo](https://docs.hyperwheel.app/es/screens/connect-a-device/) desde el paso del código QR.

## Iniciar con el sistema

**Launch on boot** está activado de forma predeterminada. En Android 10 y posteriores, iniciar con el sistema también requiere permitir **Display over other apps** para HyperWheel Player. El panel de ajustes muestra si está permitido y abre por ti la pantalla de Android correspondiente.

## Actualizaciones

- **Windows, macOS y Linux:** la aplicación busca una versión nueva al iniciarse y la instala automáticamente.
- **Android, Google TV y Fire TV:** la aplicación busca cada pocas horas. Cuando hay una versión nueva, **Actions** en el panel de ajustes muestra un punto y una fila **Install**. Android te pide que confirmes la instalación. Nada interrumpe la reproducción hasta que elijas instalar.

## Relacionado

- [Ajustes del reproductor y mando a distancia](player-settings.md)
- [Conectar un dispositivo](https://docs.hyperwheel.app/es/screens/connect-a-device/)
- [Pantalla sin conexión](https://docs.hyperwheel.app/es/troubleshooting/screen-offline/)
