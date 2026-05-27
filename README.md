# Éxito · Click to Pay — Demo visual

Demo visual de una implementación de **Click to Pay** con **Unified Checkout Solutions** sobre el checkout de exito.com, siguiendo la *Click to Pay CX Guide* de Mastercard.

🔗 **Demo en vivo:** https://linacastrillon.github.io/exito-c2p/

## Contenido

- **`index.html`** — Demo del checkout con el flujo completo, del carrito a la finalización del pago.
- **`Exito-ClickToPay-Demo.html`** — Presentación complementaria (slides).

## Casos de uso

1. **Nuevo usuario** — alta y vinculación de tarjeta.
2. **Reconocido por correo / teléfono** — `idLookup` + OTP (`initiateValidation` / `validate`).
3. **Usuario reconocido** — `isRecognized` + listado de tarjetas (`getCards`).
4. **Agregar nueva tarjeta** — `encryptCard` / `checkoutWithNewCard`.

Cada paso destaca los métodos de JavaScript/API de Unified Checkout y del SDK de SRC (EMVCo) involucrados.
