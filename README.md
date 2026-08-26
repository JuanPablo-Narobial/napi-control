# napi-control

Estado público de disponibilidad para NAPI Explorer.

El fichero `status.json` se publica con GitHub Pages y lo consulta la extensión al
seleccionar un servidor DMS. No contiene secretos, credenciales ni permisos.

## Cambiar el estado

- Para detener el uso: establecer `enabled` en `false` y añadir un `message`.
- Para obligar a actualizar: subir `minimumVersion`; bloquea todas las versiones
  inferiores.
- Para revocar una versión concreta: añadirla a `blockedVersions`.

La autorización real permanece en el backend DMS; este repositorio solo controla la
disponibilidad de la extensión distribuida.
