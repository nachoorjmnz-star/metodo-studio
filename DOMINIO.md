# Conectar el dominio metodostudio.com

La web ya está online en `https://nachoorjmnz-star.github.io/metodo-studio/`.
Para que se vea en **https://metodostudio.com** solo faltan 3 pasos. La parte técnica está toda aquí lista; tú solo compras el dominio.

---

## Paso 1 — Comprar el dominio (~10-12 €/año)
Cualquiera de estos registradores vale (elige el más barato para `.com`):
- **Porkbun** — porkbun.com
- **Namecheap** — namecheap.com
- **Dinahosting / IONOS** (españoles, soporte en español)

Compra: **metodostudio.com**

## Paso 2 — Añadir estos registros DNS
En el panel de tu registrador, en la zona **DNS**, crea exactamente estos registros:

**Para `metodostudio.com` (dominio raíz) → 4 registros tipo A:**
```
Tipo  Nombre  Valor
A     @       185.199.108.153
A     @       185.199.109.153
A     @       185.199.110.153
A     @       185.199.111.153
```

**Recomendado también, 4 registros tipo AAAA (IPv6):**
```
AAAA  @  2606:50c0:8000::153
AAAA  @  2606:50c0:8001::153
AAAA  @  2606:50c0:8002::153
AAAA  @  2606:50c0:8003::153
```

**Para que `www.metodostudio.com` también funcione → 1 registro CNAME:**
```
Tipo   Nombre  Valor
CNAME  www     nachoorjmnz-star.github.io.
```

> Si el registrador ya trae registros por defecto en `@` (una IP de aparcamiento), bórralos y deja solo estos.

## Paso 3 — Activarlo (me avisas y lo hago yo)
Cuando tengas el dominio comprado y los DNS puestos, **dímelo** y yo en 2 minutos:
1. Añado el archivo `CNAME` al repositorio con el contenido `metodostudio.com`.
2. Configuro el dominio en GitHub Pages y activo **HTTPS**.
3. Actualizo las etiquetas de la web (`og:url`, imagen social) al nuevo dominio.

Si prefieres hacerlo tú: en GitHub → repo **metodo-studio** → **Settings → Pages → Custom domain**, escribe `metodostudio.com`, guarda, espera a que verifique y marca **Enforce HTTPS**.

---

### Notas
- La propagación de los DNS tarda entre 15 minutos y unas horas (a veces hasta 24 h). Es normal.
- El dominio raíz `metodostudio.com` será el principal; `www` redirige a él.
- **Correo:** con el dominio podrás crear `hola@metodostudio.com` (la web ya usa esa dirección). Muchos registradores ofrecen redirección de correo gratis, o puedes usar Zoho Mail (gratis) / Google Workspace.
