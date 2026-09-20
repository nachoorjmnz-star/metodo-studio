# Cobrar en Método

La tienda ya está lista para vender. Solo falta conectar una pasarela que **cobre y entregue el archivo** automáticamente. Con productos digitales, lo más fácil es una plataforma que hace las dos cosas.

## Recomendado: Gumroad o Lemon Squeezy
Las dos entregan el archivo solas tras el pago y **gestionan el IVA europeo** por ti (importante vendiendo en la UE).

| | Gumroad | Lemon Squeezy | Stripe Payment Links |
|--|--------|----------------|----------------------|
| Entrega el archivo sola | ✅ | ✅ | ❌ (solo cobra) |
| Gestiona IVA UE | ✅ | ✅ | Manual |
| Comisión aprox. | ~10 % | ~5 % + fee | ~1,5 % + 0,25 € |
| Ideal para | Empezar rápido | Escalar | Ya tienes web propia |

**Sugerencia:** empieza con **Gumroad** (más simple). Si creces, pásate a Lemon Squeezy por comisión.

## Pasos
1. Crea la cuenta (Gumroad / Lemon Squeezy).
2. Sube cada producto de la carpeta `productos/` (ver cómo empaquetarlos en `productos/GUIA-DE-USO.md`).
3. Pon el precio del catálogo (ver `README.md`).
4. Copia el **enlace de compra** de cada producto.
5. Pégalos en `index.html`, en el bloque `CONFIG.enlacesPago` (arriba del `<script>`):

```js
const CONFIG = {
  moneda: "€",
  enlacesPago: {
    "control-total":       "https://tutienda.gumroad.com/l/control-total",
    "libertad-freelance":  "https://tutienda.gumroad.com/l/libertad",
    "reto-52-semanas":     "https://tutienda.gumroad.com/l/reto52",
    "segundo-cerebro":     "https://tutienda.gumroad.com/l/segundo-cerebro",
    "planner-2026":        "https://tutienda.gumroad.com/l/planner-2026",
    "habitos":             "https://tutienda.gumroad.com/l/habitos",
    "calendario-contenido":"https://tutienda.gumroad.com/l/calendario",
    "cliente-crm":         "https://tutienda.gumroad.com/l/cliente",
    "pack-todo":           "https://tutienda.gumroad.com/l/pack"
  }
};
```

6. Guarda y listo: al pulsar **Finalizar compra**, la tienda abre el enlace de pago del producto.

## Cómo funciona el carrito
Al ser productos digitales, cada uno se entrega por su propio enlace seguro. Si el cliente tiene varios en la cesta, la tienda abre el primero y le sugiere comprar el resto (o llevarse el **Pack completo**, que es más barato). Es el comportamiento normal en tiendas de plantillas.

> Mientras no pegues los enlaces, el botón muestra un aviso explicando que la tienda está lista pero faltan las claves de pago. Nada se rompe.

## ⚠️ Lo que no puedo hacer yo
Crear la cuenta de la pasarela y conectar tu banco es **tuyo** (requiere tus credenciales y datos fiscales). Yo dejo todo enchufado para que solo pegues los enlaces.
