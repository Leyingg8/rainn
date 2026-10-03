# Pendiente: activar envío de correo del formulario

Estado: el HTML ya está cableado pero **NO funciona todavía**.
Archivo: `code.html` (sección `#quote-section`, formulario `#inspection-form`).

## Por qué no llega correo todavía

`code.html` ~línea 755 tiene un endpoint de ejemplo:

```html
action="https://formspree.io/f/TU_ID_DE_FORMSPREE"
```

Ese texto es un placeholder. Mientras no se reemplace, el `fetch` falla,
Formspree devuelve error, el visitante ve el mensaje rojo
*"Something went wrong. Please call us directly at (619) 555-0199."*
y **no llega ningún correo a ninguna parte**.

## Pasos para activarlo (cuando haya acceso a la cuenta)

1. Entrar a <https://formspree.io> y crear cuenta.
2. **New Form** → dominio `https://rainorshineroofingsd.com` → **Create Form**.
3. En **Settings**:
   - **Notifications**: agregar `eric@rainorshineroofingsd.com` como destinatario.
   - Activar **"Enable file attachments"** (sin esto el campo `photos` llega vacío).
   - Campo *Subject*: `_subject` (para que use el asunto que ya trae el hidden input).
4. Copiar el ID del endpoint (ej. `xpwzgrqv`) y reemplazar `TU_ID_DE_FORMSPREE`
   en `code.html`.

## Límite de archivos

La etiqueta del formulario dice 10MB por archivo porque ese es el tope de
Formspree. Si se sube un archivo mayor, el JS lo rechaza antes de enviar.

## Campos enviados (ya configurados con `name`)

`name`, `phone`, `email`, `service_type`, `property_address`, `photos`, `notes`