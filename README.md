# SmartTank · Descarga

Página de descarga de **SmartTank**, sistema IoT de monitoreo del nivel de agua en tanques domésticos (ESP32 + sensor ultrasónico HC-SR04 + app Flutter).

Proyecto de grado · Ingeniería Informática · Corporación Universitaria Autónoma de Nariño, extensión Villavicencio.

## Contenido

| Archivo | Descripción |
|---|---|
| `index.html` | Landing page (HTML, CSS y JS en un solo archivo) |
| `SmartTank.apk` | APK de Android que descarga el botón |
| `img/` | Ícono y capturas de la app |

## Publicar una versión nueva del APK

1. En `smarttank-app`, compila: `flutter build apk --release --target-platform android-arm,android-arm64`
2. Copia `build/app/outputs/flutter-apk/app-release.apk` a este repositorio como `SmartTank.apk` (reemplazando el anterior).
3. En `index.html`, actualiza la versión y el tamaño en la línea `const APK = { version: "...", tamanoMB: ... };`
4. Haz commit y push. GitHub Pages publica los cambios en uno o dos minutos.
