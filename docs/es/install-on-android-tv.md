# Instalar en Google TV y Android TV

_Instala la aplicación HyperWheel Player en Google TV, Android TV y cajas Android TV con Downloader, Send Files to TV o ADB._

> **Probada en:** un emulador de Google TV con Android 14, incluidas las pantallas de instalación, el panel de ajustes con un mando, el inicio con el sistema y las actualizaciones. Aún no se ha probado en un televisor ni en una caja reales. Los nombres de los menús cambian según el fabricante y la versión de Android.

## Qué necesitas

- un dispositivo Google TV, Android TV o Chromecast con Google TV, o una caja Android TV, con Android 7 o posterior
- conexión a internet
- una forma de pasar el archivo al televisor: la aplicación Downloader, Send Files to TV o ADB

Para Fire TV, consulta la guía de Fire TV.

## 1. Permitir instalaciones fuera de Play Store

1. Abre **Configuración**, luego **Sistema** y **Información**.
2. Selecciona **Compilación de Android TV OS** (o **Compilación**) siete veces hasta que un mensaje indique que ya eres desarrollador.
3. Vuelve a **Configuración**, luego **Aplicaciones**, **Seguridad y restricciones** y **Orígenes desconocidos**. Activa la aplicación con la que abrirás el archivo (Downloader o Archivos de Google).

En Android 8 y posteriores, Android puede pedirte que lo permitas la primera vez que abras el archivo.

## 2. Llevar la aplicación al televisor

Elige una opción.

**Downloader (la más rápida con un mando)**

1. Instala **Downloader** desde Google Play Store en el televisor.
2. Ábrela y escribe **hypr.onl/get** en la barra de direcciones. Selecciona **Go**.
3. Cuando termine la descarga, selecciona **Install** y luego **Done**.

**Send Files to TV**

1. Instala **Send Files to TV** en el televisor y en tu teléfono.
2. Envía el archivo `HyperWheel-Player_latest_android.apk` desde tu teléfono al televisor.
3. Abre el archivo en el televisor y selecciona **Instalar**.

**ADB**

1. En **Opciones para desarrolladores**, activa **Depuración por USB** (o **Depuración inalámbrica**) y anota la dirección IP del televisor.
2. En un ordenador:

```sh
adb connect <direccion-ip-del-televisor>:5555
adb install -r HyperWheel-Player_latest_android.apk
```

## 3. Abrir la aplicación

Busca **HyperWheel Player** en tu fila de aplicaciones. Muestra **Link this screen** con un código QR. Sigue [Conectar un dispositivo](https://docs.hyperwheel.app/es/screens/connect-a-device/) desde el paso del código QR. Pulsa **OK** en el mando para abrir el panel de ajustes.

## Iniciar con el sistema

**Launch on boot** está activado de forma predeterminada. Android 10 y posteriores también necesitan **Display over other apps** para la aplicación:

1. Abre el panel de ajustes y busca en **Settings**. La fila **Display over other apps** muestra **Not allowed**.
2. Pulsa **OK** en ella. Android abre **Permitir mostrar sobre otras aplicaciones**. Activa **HyperWheel Player** y pulsa **Atrás**.

Si un televisor no tiene esa pantalla, usa ADB:

```sh
adb shell appops set app.hyperwheel.player SYSTEM_ALERT_WINDOW allow
```

La aplicación también se reinicia sola si se detiene de forma inesperada. Lo hace como máximo tres veces en diez minutos, para que un fallo repetido no pueda mantener ocupado el televisor.

## Mando a distancia

- **OK** abre el panel de ajustes. Las flechas se mueven y **OK** selecciona.
- **Atrás** cierra el panel paso a paso. Con el panel cerrado, **Atrás** no hace nada, así que una pulsación accidental nunca saca al reproductor.
- Para salir de la aplicación, **mantén pulsado Atrás** durante tres segundos. **Inicio** también sale de ella.
- Si tu mando tiene un botón **Menú**, también abre el panel de ajustes.

## Actualizar

La aplicación busca una versión nueva cada pocas horas. Cuando hay una lista, **Actions** muestra un punto. Abre **Actions**, selecciona **Install** y confirma con el mando. La primera vez, permite **Instalar aplicaciones desconocidas** para HyperWheel Player cuando Android lo pida.

## Desinstalar

Abre **Configuración**, luego **Aplicaciones**, selecciona **HyperWheel Player** y después **Desinstalar**.

## Solución de problemas

- **La primera pulsación de OK no hace nada justo después de abrir la aplicación.** Púlsalo de nuevo.
- **La aplicación no se inicia tras un corte de luz.** Permite **Display over other apps**, como se indica arriba.
- **El vídeo se ve mal o la aplicación no se inicia en una caja con un sistema antiguo.** Abre **Configuración**, **Aplicaciones**, **Android System WebView** y actualízalo desde Play Store si puedes. Si la caja no se puede actualizar, no es compatible.
- **La pantalla se queda en Link this screen.** Consulta [Conectar un dispositivo](https://docs.hyperwheel.app/es/screens/connect-a-device/).
