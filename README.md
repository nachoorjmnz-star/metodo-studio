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
| Planner 2026 (imprimible) | Productividad | 19 € | 29 € |
| Hábitos (tracker) | Productividad | 12 € | 18 € |
| Calendario de Contenido | Creadores | 24 € | 34 € |
| Cliente (CRM ligero) | Creadores | 34 € | 44 € |
| **Pack completo "Todo Método"** | Pack | **89 €** | 195 € |

Estrategia de precio: producto gancho a 9 €, flagship a 29 €, y **pack a 89 €** como ancla (ahorro del 54 %) para subir el ticket medio.

## 4. Qué está construido (por mí, listo)

- `index.html` — tienda completa y autónoma: catálogo con filtros, vista rápida de cada producto, **carrito con localStorage**, pack destacado, cómo funciona, reseñas (marcadas como ilustrativas), FAQ, newsletter, footer. Responsive (móvil/tablet/PC). SEO + Open Graph + datos estructurados.
- `productos/` — **los productos de verdad**, creados por mí:
  - 6 plantillas de hoja de cálculo (`.csv`) en español, listas para Google Sheets/Excel.
  - `segundo-cerebro.md` — sistema Notion listo para pegar.
  - `planner-2026.html` — planner imprimible a PDF (calendario 2026 correcto, genera 12 meses + semanal + metas).
  - `GUIA-DE-USO.md` — cómo empaquetar cada uno para venderlo.
- Guías: `PAGOS.md`, `DESPLIEGUE.md`, `MARKETING.md`.

## 5. Qué falta (depende de ti — no lo puedo hacer por norma)

Son cosas que requieren **tus cuentas o credenciales**:

1. **Cobrar:** crear cuenta en **Gumroad** o **Lemon Squeezy** (recomendado para digital + IVA europeo), subir cada producto y pegar los enlaces en `CONFIG.enlacesPago` dentro de `index.html`. → ver `PAGOS.md`.
2. **Publicar la web:** cuenta de **Netlify** (arrastrar la carpeta) o `gh` autenticado y yo la subo a GitHub Pages. → ver `DESPLIEGUE.md`.
3. **Redes:** crear las cuentas TikTok/Instagram de la marca (guiones listos en `MARKETING.md`).
4. **Alta legal** para vender (autónomo/formas de facturar).

## 6. Fuentes del estudio

- Sellfy — https://sellfy.com/blog/digital-products/
- Amasty — https://amasty.com/blog/best-digital-products-to-sell/
- SendOwl (categorías que más venden) — https://www.sendowl.com/blog/tips-and-advice/best-selling-notion-template-categories
- Biztoolkit (ingresos de creadores) — https://www.biztoolkit.co/post/how-much-do-notion-template-creators-make-in-2026
- Etsy trends 2026 — https://www.sellerapp.com/blog/etsy-trends/

---
_Proyecto personal · fuera del TFG. Reseñas y datos de ejemplo son ilustrativos de una tienda de demostración._
