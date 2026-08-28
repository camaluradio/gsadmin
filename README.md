# GS💊ADMIN Android 1.0.0

Proyecto Android completo para compilar GS💊ADMIN desde cero con GitHub Actions.

## Comportamiento de conexión
- Con Internet: WebView normal.
- Sin Internet: se detiene la carga y se muestra exclusivamente la pantalla offline.
- Al recuperar Internet: vuelve a cargar GS💊ADMIN automáticamente y sin mostrar avisos de reconexión.
- No existe modo consulta/caché offline.

## Push
Firebase Cloud Messaging permanece activo y suscripto al topic `gsadmin-alertas`.
El token FCM no se muestra ni se copia al portapapeles.

## GitHub
Subir el CONTENIDO de esta carpeta a la raíz del repositorio y ejecutar Actions > Generar APK GS ADMIN.
El artefacto resultante se llama `GS-ADMIN-1.0.0.apk`.

IMPORTANTE: no subir al repositorio ninguna clave privada de Firebase Admin / service account.
