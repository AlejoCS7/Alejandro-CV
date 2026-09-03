# Alejandro Caicedo Sanguino — CV / Currículum

CV interactivo de una sola página, **bilingüe (Español / English)**, publicado como sitio estático.
Diseño oscuro tipo *command center*, con animaciones sutiles, línea de tiempo de experiencia
en acordeón y un pequeño *easter egg* en pixel-art.

🔗 **Sitio:** https://TU-USUARIO.github.io/NOMBRE-DEL-REPO/

---

## ✨ Características

- **Toggle de idioma ES / EN** en la barra de navegación (visible también en móvil).
  - Autodetecta el idioma del navegador en la primera visita.
  - Recuerda la elección del visitante (`localStorage`).
  - Enlace directo por idioma: `.../#es` o `.../#en`.
- **Un solo archivo autocontenido** — todo el CSS y JavaScript va embebido; las tipografías
  se cargan por CDN de Google Fonts. No hay dependencias que instalar ni compilar.
- **Accesible** — navegación por teclado en el acordeón (Enter / Espacio), `aria-expanded`,
  `aria-label` traducidos y soporte de `prefers-reduced-motion`.
- **Responsivo** — se adapta de escritorio a móvil; los elementos decorativos pesados
  (circuito animado, bombilla) se ocultan en pantallas pequeñas.
- **SEO básico** — `<title>` y `meta description` propios, que además cambian con el idioma.

## 🗂️ Estructura

```
index.html      # Sitio publicado (punto de entrada de GitHub Pages)
```

> El repositorio solo necesita `index.html`. Todo lo demás (estilos, scripts, íconos SVG)
> vive dentro de ese archivo.

## 🚀 Publicar en GitHub Pages

1. Sube `index.html` a un repositorio público.
2. Ve a **Settings → Pages**.
3. En *Source* elige **Deploy from a branch** → rama `main` → carpeta `/ (root)` → **Save**.
4. En 1–2 minutos el sitio estará disponible en la URL de arriba.

> Para servirlo en la raíz (`https://TU-USUARIO.github.io/`), nombra el repositorio
> exactamente `TU-USUARIO.github.io`.

## ✏️ Editar el contenido

Cada texto traducible lleva sus dos idiomas juntos en el mismo elemento, por ejemplo:

```html
<li data-en="Accelerated permit approval timelines…"
    data-es="Aceleré los tiempos de aprobación de permisos…">…</li>
```

Edita el par `data-en` / `data-es` y el idioma activo se muestra automáticamente.
Así ambas versiones se mantienen sincronizadas con un solo cambio.

## 🛠️ Desarrollo local

Al ser un archivo estático, basta con abrirlo en el navegador. Para servirlo localmente:

```bash
python -m http.server 8000
# luego abre http://localhost:8000
```

## 📬 Contacto

- ✉️ darioc97@gmail.com
- 📱 +57 316 389 4235
- 💼 [LinkedIn](https://www.linkedin.com/in/alejandro-caicedo-sanguino-006a5a151)
- 📍 Bogotá, Colombia
