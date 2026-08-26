# napi-control

## Cambiar el estado

- Para detener el uso: establecer `enabled` en `false` y añadir un `message`.
- Para obligar a actualizar: subir `minimumVersion`; bloquea todas las versiones
  inferiores.
- Para revocar una versión concreta: añadirla a `blockedVersions`.

La autorización real permanece en el backend DMS; este repositorio solo controla la
disponibilidad de la extensión distribuida.
