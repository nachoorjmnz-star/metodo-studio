# Poner Método online

La tienda es un sitio estático (un `index.html` + la carpeta `productos/`). Se publica en segundos y **gratis**.

## Opción A — Netlify Drop (la más fácil, sin cuenta técnica)
1. Entra en **https://app.netlify.com/drop**.
2. Arrastra la carpeta `metodo-studio` entera a la página.
3. Te da una URL pública al momento (ej: `metodo-studio.netlify.app`).
4. Para dominio propio: en Netlify → *Domain settings* → añade tu dominio.

## Opción B — GitHub Pages (si usas `gh`)
Si vuelves con GitHub autenticado (`gh auth login`), **yo lo despliego**:
1. Creo un repo público con el contenido.
2. Activo GitHub Pages sobre la rama principal.
3. Queda en `https://<tu-usuario>.github.io/metodo-studio/`.

## Opción C — Vercel
Similar a Netlify: `vercel` en la carpeta, o conecta el repo de GitHub.

## Dominio (opcional pero recomendable)
Un dominio corto da confianza y ayuda a las ventas:
- Ideas: `metodo.studio`, `metodoplantillas.com`, `usametodo.com`.
- Cómpralo en Namecheap / Porkbun / IONOS (~10 €/año) y apúntalo a Netlify.

## Antes de abrir al público (checklist)
- [ ] Enlaces de pago pegados en `CONFIG.enlacesPago` (ver `PAGOS.md`).
- [ ] Productos subidos a la pasarela y probados con una compra de prueba.
- [ ] Rellenar páginas legales (Términos, Privacidad, Reembolsos) — obligatorio vendiendo.
- [ ] Cambiar el email `hola@metodo.studio` por el tuyo real de la marca.
- [ ] Newsletter conectada (Mailchimp/MailerLite) si quieres regalar la plantilla gratis.

## ⚠️ Lo que no puedo hacer yo
Crear la cuenta de hosting o comprar el dominio (requiere tus credenciales/pago). Con `gh` autenticado, el despliegue en GitHub Pages sí lo hago yo.
