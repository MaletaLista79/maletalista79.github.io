# Maleta Lista — web

Página web de **Maleta Lista**, servicio de itinerarios de viaje a medida.

Está hecha solo con HTML y CSS (nada que instalar, ninguna dependencia externa).
Se publica gratis en GitHub Pages.

- Dirección final prevista: **https://maletalista79.github.io/**
- Perfil de Fiverr al que apuntan todos los botones: https://www.fiverr.com/maletalista

---

## 1. Qué archivo es cada cosa

| Archivo | Para qué sirve |
|---|---|
| `index.html` | **El contenido**: todos los textos, secciones y enlaces. Si quieres cambiar una frase o un precio, es aquí. |
| `styles.css` | **El aspecto**: colores, tamaños, márgenes. Los colores están todos juntos al principio del archivo. |
| `assets/logo.svg` | El logotipo completo (maleta + nombre). |
| `assets/favicon.svg` | El iconito que sale en la pestaña del navegador. |
| `README.md` | Este manual. No se ve en la web. |

> **SVG** es un formato de imagen hecho con texto en lugar de puntos de color.
> Por eso se ve nítido en cualquier tamaño y pesa muy poco.

---

## 2. Cómo ver la web en tu ordenador (Windows)

La forma más rápida:

1. Abre el **Explorador de archivos** (la carpeta amarilla de la barra de tareas).
2. Ve a `Descargas` → `maletalista`.
3. **Haz doble clic en `index.html`.**

Se abrirá en tu navegador y verás la web. Fíjate en que arriba, en la barra de
direcciones, aparece algo como `file:///C:/Users/...`: eso significa que la estás
viendo desde tu disco duro, no desde internet. Solo la ves tú.

Si al hacer doble clic se abre otro programa (por ejemplo el Bloc de notas):
haz **clic derecho** sobre `index.html` → **Abrir con** → **Google Chrome**
(o Edge, o Firefox).

### Probar cómo se ve en el móvil sin tener móvil

1. Con la web abierta en Chrome o Edge, pulsa la tecla **F12**.
2. Se abre un panel con código. Pulsa **Ctrl + Mayúsculas + M**.
3. La página se verá dentro de un marco estrecho, como en un teléfono. Arriba
   puedes elegir el modelo (iPhone, Galaxy...).
4. Para salir, pulsa **F12** otra vez.

### Si cambias un texto y no ves el cambio

Guarda el archivo y pulsa **Ctrl + F5** en el navegador (recarga forzando la
descarga de todo de nuevo).

---

## 3. Cómo publicarla en internet con GitHub Pages

**Qué es esto.** GitHub es una web donde se guardan archivos de programación.
GitHub Pages es un servicio suyo, gratuito, que convierte una carpeta de
archivos en una web pública. No hay que pagar nada ni instalar nada, y todo se
hace desde el navegador. No necesitas escribir ni un comando.

Un **repositorio** (o "repo") es simplemente una carpeta dentro de GitHub.

Tu usuario es `MaletaLista79`.

### Paso 1 — Crear el repositorio con el nombre exacto

1. Entra en https://github.com e inicia sesión con tu cuenta `MaletaLista79`.
2. Arriba a la derecha, pulsa el botón **+** y elige **New repository**
   (*nuevo repositorio*).
3. Rellena así:
   - **Repository name**: escribe exactamente
     ```
     maletalista79.github.io
     ```
     ⚠️ Todo en minúsculas y con el punto. **El nombre tiene que ser tu usuario
     seguido de `.github.io`**. Si lo escribes con otro nombre, la web no saldrá
     en la dirección corta.
   - **Description**: puedes dejarlo vacío o poner "Web de Maleta Lista".
   - Marca **Public** (*público*). Tiene que ser público para que Pages
     funcione gratis.
   - **No marques** "Add a README file" ni ninguna otra casilla de abajo.
4. Pulsa el botón verde **Create repository**.

### Paso 2 — Subir los archivos arrastrándolos

1. En la página que acaba de aparecer, busca el enlace
   **uploading an existing file** (*subir un archivo existente*). Está en el
   texto de la zona central. Púlsalo.
   *Si no lo encuentras:* pulsa el botón **Add file** → **Upload files**.
2. Abre en otra ventana tu carpeta `Descargas\maletalista`.
3. Selecciona `index.html`, `styles.css`, `README.md` **y la carpeta `assets`**
   (puedes marcarlos con el ratón manteniendo **Ctrl** pulsado).
4. **Arrástralos** a la zona de GitHub que dice
   *"Drag files here to add them to your repository"*.

   ⚠️ **Importante:** arrastra la carpeta `assets` entera, no los dos SVG
   sueltos. Si subes los SVG sueltos, el logo no aparecerá, porque la página los
   busca dentro de `assets/`.

   **No subas** las carpetas `.cursor`, `skills` ni `examples`, ni el archivo
   `AGENTS.md`: son notas de trabajo, no forman parte de la web.
5. Espera a que terminen de subirse (aparecerán listados con su nombre).
6. Baja hasta el recuadro **Commit changes**. En el campo de arriba escribe una
   nota corta, por ejemplo `Primera versión de la web`.

   > Un **commit** es "guardar una versión". GitHub conserva todas, así que
   > nunca pierdes lo anterior.
7. Pulsa el botón verde **Commit changes**.

### Paso 3 — Encender GitHub Pages

1. En la barra de arriba del repositorio, pulsa **Settings** (*ajustes*,
   con un icono de engranaje).
2. En la columna de la izquierda, busca y pulsa **Pages**.
3. En el apartado **Build and deployment** → **Source**, deja seleccionado
   **Deploy from a branch** (*publicar desde una rama*).
4. Justo debajo, en **Branch**, hay dos desplegables:
   - En el primero elige **main**.
   - En el segundo deja **/ (root)**.
5. Pulsa **Save** (*guardar*).

### Paso 4 — Esperar y comprobar

- GitHub tarda entre **1 y 5 minutos** la primera vez.
- Recarga la página de **Settings → Pages**. Cuando esté lista aparecerá un
  recuadro verde con tu dirección:
  ```
  https://maletalista79.github.io/
  ```
- Ábrela. Si ves la web, ya está publicada y cualquiera puede entrar.

> **Si ves una página en blanco o un error 404** (página no encontrada):
> espera dos minutos más y recarga con **Ctrl + F5**. Si sigue igual, comprueba
> en el repositorio que el archivo se llama `index.html` en minúsculas y que
> está en la raíz, no dentro de otra carpeta.
>
> **Si la web sale pero sin colores:** es que `styles.css` no se subió o se
> subió con otro nombre.
>
> **Si no sale el logo:** es que los SVG no están dentro de la carpeta `assets`.

### Paso 5 — Cómo cambiar algo más adelante

Siempre desde la web de GitHub, sin instalar nada:

1. Entra en tu repositorio y pulsa sobre el archivo que quieras cambiar
   (por ejemplo `index.html`).
2. Pulsa el icono del **lápiz** (arriba a la derecha del archivo).
3. Haz el cambio, baja y pulsa **Commit changes**.
4. En 1-2 minutos la web pública se actualiza sola.

Para subir un archivo nuevo o reemplazar uno: **Add file** → **Upload files**.
Si subes un archivo con el mismo nombre, sustituye al anterior.

---

## 4. Cómo cambiar los colores

Abre `styles.css`. Al principio verás esto:

```css
:root {
  --petroleo: #0f5c6b;   /* color principal */
  --amarillo: #ffd166;   /* acentos y botones destacados */
  --crema: #f6efe3;      /* fondo */
  --tinta: #222222;      /* texto */
}
```

Cambia un código de color ahí y cambia en toda la web de golpe.
Los códigos tipo `#0f5c6b` se pueden elegir en https://htmlcolorcodes.com/es/

---

## 5. Pendiente para más adelante (opcional)

- **Imagen para compartir en redes.** Ahora, al pegar el enlace en WhatsApp o
  Facebook, se usa el logo. Queda mejor una foto horizontal de 1200 × 630
  píxeles. Cuando la tengas, guárdala como `assets/portada.jpg` y en
  `index.html` cambia las dos líneas que contienen `og:image` y `twitter:image`
  para que apunten a `https://maletalista79.github.io/assets/portada.jpg`.
- **Dominio propio** (por ejemplo `maletalista.com`): se puede conectar a
  GitHub Pages desde **Settings → Pages → Custom domain**.
- **Enlaces de afiliados y redes sociales:** ya hay un hueco preparado y
  explicado al final de `index.html`, dentro del pie de página.
- **Aviso legal y privacidad:** hacen falta en España si algún día recoges datos
  (formularios, suscripción) o usas enlaces de afiliados.
