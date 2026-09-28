# Método — tienda de plantillas digitales

**Sistemas para ordenar tu dinero, tu tiempo y tus metas.**
Tienda online de productos digitales (finanzas + productividad) en español. Hecha entera de forma autónoma: estudio de mercado, nicho, marca, catálogo, precios, diseño y los propios productos.

📄 Abre `index.html` en el navegador para ver la tienda.

---

## 1. Estudio de mercado (por qué este nicho)

Investigué tres frentes (fuentes abajo) antes de decidir nada:

| Hallazgo | Fuente |
|----------|--------|
| Los **productos digitales** tienen márgenes del **70–95 %** (sin stock, sin envíos, sin proveedor). | Sellfy, Amasty |
| Las 4 categorías que se llevan **~2/3 de las ventas**: **finanzas personales, sistemas de productividad, calendarios de contenido y CRMs ligeros**. | SendOwl |
| Los creadores de plantillas ganan **500–15.000 €/mes**; los de **finanzas** son los que más (10.000–25.000 €/mes). Precios típicos **5–49 €**, packs premium **79–199 €**. | Biztoolkit, SendOwl |
| Lo que vende no es lo genérico, sino lo **específico de un nicho** (para freelancers, para creadores…). | Etsy trends, Inkfluence |

**Decisión y por qué es inteligente:**
1. **Modelo = productos digitales.** Esquiva el muro que frenó las otras dos tiendas (necesitar fotos de proveedor de AliExpress, envíos y pasarela). Aquí **los productos los he creado yo**, así que la tienda nace con catálogo real.
2. **Nicho = finanzas + productividad**, las categorías más rentables y con más demanda.
3. **En español.** Los referentes (Easlo, Thomas Frank…) son todos en inglés → el mercado hispano está **menos saturado**. Es la ventaja de "nicho específico".
4. **Distinto de tus otras tiendas** (Lumé Studio = hogar; VYRAL = gadgets virales). Sin solapamiento.

## 2. La marca

- **Nombre:** Método — dice literalmente lo que vende (un método/sistema).
- **Eslogan:** *Ordena tu dinero, tu tiempo y tus metas.*
- **Tono:** cercano, práctico, "menos apps y menos ansiedad".
- **Estética:** editorial papel + tinta, acento verde pino (confianza/calma/finanzas). Tipografías Fraunces (serif) + Inter.

## 3. Catálogo y precios

| Producto | Categoría | Precio | Antes |
|----------|-----------|-------:|------:|
| Control Total (panel de finanzas) | Finanzas | 29 € | 39 € |
| Libertad (finanzas freelance) | Finanzas | 39 € | 49 € |
| Reto 52 Semanas (ahorro) | Finanzas | 9 € | 14 € |
| Segundo Cerebro (Notion) | Productividad | 29 € | 39 € |
| Planner 2026 (PDF hiperenlazado) | Productividad | 19 € | 29 € |
| Hábitos (tracker) | Productividad | 12 € | 18 € |
| Calendario de Contenido | Creadores | 24 € | 34 € |
| Cliente (CRM ligero) | Creadores | 34 € | 44 € |
| **Pack completo "Todo Método"** | Pack | **89 €** | 195 € |

Estrategia de precio: producto gancho a 9 €, flagship a 29 €, y **pack a 89 €** como ancla (ahorro del 54 %) para subir el ticket medio.

## 4. Qué hay en este repositorio (la web pública)

- `index.html` — la tienda: catálogo con filtros, ficha de cada producto («qué incluye» y «lo que recibes»), carrito, pack, garantías, FAQ, plantilla gratis y footer. Responsive, con SEO, Open Graph y datos estructurados de producto.
- `guia.html` — guía de instalación para clientes (Excel, Google Sheets, Numbers, Notion, iPad).
- `terminos.html`, `privacidad.html`, `reembolsos.html` — legales (faltan tus datos: `[NOMBRE]`, `[NIF]`, `[DIRECCIÓN]`).
- `gratis/` — la plantilla gratuita (Mini-presupuesto), descargable desde la web.
- `img/` y `og.png` — imágenes para buscadores y redes. `404.html`, `sitemap.xml`, `robots.txt`.
- `_config.yml` — evita que los `.md` internos (este README, PAGOS, MARKETING…) se publiquen en la web.

## 5. Los productos de pago NO están aquí

Viven en la carpeta local `privado/` (ignorada por git, **nunca se publica**):

- `privado/entregables/paquetes/` — lo que se sube a Gumroad, producto a producto (+ `manifest.json` con nombres y precios).
- `privado/entregables/xlsx/` — 7 plantillas Excel con fórmulas, paneles, gráficos y desplegables (funcionan en Excel, Google Sheets y Numbers).
- `privado/entregables/pdf/` — Planner 2026 hiperenlazado (6 versiones, 86-87 páginas), láminas imprimibles y una guía rápida PDF por producto.
- `privado/entregables/notion/` — Segundo Cerebro para importar en Notion.
- `privado/entregables/portadas/` — portadas y miniaturas para Gumroad.
- `privado/herramientas/` — los generadores. Para regenerarlo todo: `python privado/herramientas/package.py`
  (y `python privado/herramientas/verify.py` tras `build_xlsx.py --verify` comprueba las fórmulas: 118/118 correctas).

## 6. Qué falta (depende de ti: cuentas y datos)

1. **Cobrar:** conectar tu banco en Gumroad (Payouts) → se publican los productos → sus enlaces van en `CONFIG.enlacesPago` de `index.html` (y el del producto gratis en `CONFIG.enlaceGratis`). → ver `PAGOS.md`.
2. **Dominio:** comprar `metodostudio.com` y seguir `DOMINIO.md`.
3. **Legal:** tus datos en las páginas legales y el alta para vender.
4. **Redes:** cuentas de TikTok/Instagram (guiones en `MARKETING.md`).

## 7. Fuentes del estudio

- Sellfy — https://sellfy.com/blog/digital-products/
- Amasty — https://amasty.com/blog/best-digital-products-to-sell/
- SendOwl (categorías que más venden) — https://www.sendowl.com/blog/tips-and-advice/best-selling-notion-template-categories
- Biztoolkit (ingresos de creadores) — https://www.biztoolkit.co/post/how-much-do-notion-template-creators-make-in-2026
- Etsy trends 2026 — https://www.sellerapp.com/blog/etsy-trends/

---
_Proyecto personal · fuera del TFG. Los datos que aparecen en las plantillas son ejemplos para borrar._
