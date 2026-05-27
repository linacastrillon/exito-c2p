# Éxito · Click to Pay — Demo visual

Demo visual de una implementación de **Click to Pay** con **Unified Checkout Solutions** sobre el checkout de exito.com, siguiendo la *Click to Pay CX Guide* de Mastercard.

🔗 **Demo en vivo:** https://linacastrillon.github.io/exito-c2p/

## Estructura (sitio multipágina)

El menú principal son páginas independientes que comparten `styles.css` y el mismo header:

- **`index.html`** — Inicio (portada).
- **`ventajas.html`** — Ventajas de Click to Pay.
- **`demo.html`** — Demo interactivo del checkout. La sección "Tarjeta crédito o débito" está en blanco (`#usecase-canvas`) para construir los casos de uso desde cero.
- **`metodos.html`** — Mapa de métodos JavaScript / API.
- **`styles.css`** — Estilos compartidos por todas las páginas.
- **`referencia-c2p.html`** — Archivo de referencia: flujo completo de Click to Pay (popup de bienvenida + modal con todos los casos de uso + JS) versionado desde el commit `bcab9aa`.
- **`exito_checkout_c2p.html`** — Versión original todo-en-uno (archivada).

## Casos de uso

1. **Nuevo usuario** — alta y vinculación de tarjeta.
2. **Reconocido por correo / teléfono** — `idLookup` + OTP (`initiateValidation` / `validate`).
3. **Usuario reconocido** — `isRecognized` + listado de tarjetas (`getCards`).
4. **Agregar nueva tarjeta** — `encryptCard` / `checkoutWithNewCard`.

Cada paso destaca los métodos de JavaScript/API de Unified Checkout y del SDK de SRC (EMVCo) involucrados.
