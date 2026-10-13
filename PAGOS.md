# Cobrar en Método (Gumroad)

## Estado actual

Los **10 productos ya están creados en Gumroad** (cuenta *Nacho Ortega*) como **borradores**, completos: nombre, precio en **euros**, descripción de venta, portada, miniatura y archivos.

| Producto | Precio | Enlace |
|---|---:|---|
| Control Total | 29 € | nachoorjmnz.gumroad.com/l/control-total |
| Libertad | 39 € | nachoorjmnz.gumroad.com/l/libertad |
| Reto 52 Semanas | 9 € | nachoorjmnz.gumroad.com/l/reto-52-semanas |
| Segundo Cerebro | 29 € | nachoorjmnz.gumroad.com/l/segundo-cerebro |
| Planner 2026 | 19 € | nachoorjmnz.gumroad.com/l/planner-2026 |
| Hábitos | 12 € | nachoorjmnz.gumroad.com/l/habitos |
| Calendario de Contenido | 24 € | nachoorjmnz.gumroad.com/l/calendario-contenido |
| Cliente | 34 € | nachoorjmnz.gumroad.com/l/cliente-crm |
| Todo Método (pack) | 89 € | nachoorjmnz.gumroad.com/l/todo-metodo |
| Mini-presupuesto (gratis) | 0 € | nachoorjmnz.gumroad.com/l/mini-presupuesto-gratis |

La web ya tiene estos enlaces puestos en `index.html`, detrás de un interruptor: `abierto: false`.

## Para abrir las ventas (3 pasos)

1. **Conecta el cobro (lo haces tú):** Gumroad → *Settings* → *Payments*. Elige **Spain**, marca las dos casillas (tienes DNI y puedes acreditar residencia) y añade tu **cuenta bancaria (IBAN)**. Sin esto Gumroad no deja publicar.
2. **Publica los productos:** en *Products*, entra en cada uno y pulsa **Publish** (o dímelo y lo hago yo).
3. **Abre la tienda:** en `index.html` cambia `abierto: false` por `abierto: true` y sube el cambio (o dímelo y lo hago yo).

A partir de ahí, cada botón «Comprar →» de la cesta lleva al producto en Gumroad, y la plantilla gratis pasa por Gumroad (así recoges el email de quien la descarga).

## Una decisión que es tuya: la garantía de devolución

Gumroad muestra por defecto **«30-day money back guarantee»** (ajuste de tu cuenta). Tu página `reembolsos.html` habla de **14 días** y de reembolso si algo falla. Elige una opción y las dejo coherentes:
- **A)** Garantía de 14 días (ajusta *Settings* o activa «Specify a refund policy for this product» en cada producto → 14 días).
- **B)** Sin devoluciones salvo fallo (opción «No refunds allowed») y mantener la política actual.

## Cómo funciona el carrito

Cada plantilla se entrega por su propio enlace seguro de Gumroad. Si alguien mete varias en la cesta, cada una tiene su botón «Comprar →», y se le sugiere el **Pack** (más barato). Si el pack está en la cesta, «Finalizar compra» abre directamente el pack.

## Si cambias de pasarela

Los enlaces están en `CONFIG.enlacesPago` y `CONFIG.enlaceGratis` de `index.html`. Sirve cualquier pasarela con enlace de pago por producto (Lemon Squeezy, Payhip, Stripe Payment Links).
