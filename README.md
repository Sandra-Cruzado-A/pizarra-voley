# Pizarra de vóley

Entrenos, partidos, plantilla, cuerpo técnico y progreso de tus equipos de minivoley (1º a 6º de primaria).
Funciona en el móvil como una app instalada, también sin conexión.

## Archivos

Todos van en la raíz del repositorio, sin carpetas:

| Archivo | Para qué sirve |
|---|---|
| `index.html` | La app completa |
| `manifest.webmanifest` | Nombre, colores e iconos para instalarla en el móvil |
| `sw.js` | Permite abrirla sin conexión |
| `favicon.svg`, `icon-192.png`, `icon-512.png`, `icon-maskable-512.png`, `apple-touch-icon.png` | Iconos |

## 1. Guarda tus datos de la versión de Claude

Los datos de la versión de Claude no pasan solos a GitHub. Antes de nada:

1. Abre la Pizarra en Claude.
2. Ve a **Progreso** y baja hasta el final.
3. Toca **Descargar copia de seguridad** (o **Guardar copia**). Se descarga un archivo `pizarra-voley-FECHA.json`.

## 2. Crea el repositorio

1. Entra en https://github.com/new
2. Nombre: `pizarra-voley`
3. Márcalo como **Public**. GitHub Pages gratis solo funciona con repositorios públicos. El código será visible, pero tus datos no: se guardan en tu móvil, nunca en GitHub.
4. Pulsa **Create repository**.

## 3. Sube los archivos

1. **Descomprime primero el zip** en tu ordenador. Si arrastras desde dentro del zip, GitHub puede perder archivos.
2. En el repositorio, pulsa **Add file → Upload files**.
3. Arrastra los 9 archivos de la carpeta descomprimida, este README incluido (los archivos, no la carpeta).
4. Pulsa **Commit changes**.

## 4. Activa GitHub Pages

1. En el repositorio, ve a **Settings → Pages**.
2. En **Source**, elige **Deploy from a branch**.
3. En **Branch**, elige `main` y la carpeta `/ (root)`. Pulsa **Save**.
4. Espera uno o dos minutos. La app estará en:

   **https://sandra-cruzado-a.github.io/pizarra-voley/**

## 5. Instálala en el móvil

- **Android (Chrome):** abre el enlace, toca el menú ⋮ y elige **Instalar aplicación** o **Añadir a pantalla de inicio**.
- **iPhone (Safari):** abre el enlace, toca el botón **Compartir** y elige **Añadir a pantalla de inicio**.

Aparecerá con el icono de la red y las seis posiciones, y se abrirá a pantalla completa.

## 6. Recupera tus datos

1. En la app instalada, ve a **Progreso → Datos y ajustes**.
2. Toca **Importar copia** y elige el archivo `.json` que descargaste en el paso 1.

Si empiezas de cero, en **Ejercicios** tienes el botón **Añadir 12 de ejemplo**.

## 7. Activa la IA (gratis, con Gemini)

Fuera de Claude, las ideas de ejercicios y el resumen del progreso usan Gemini:

1. Consigue una clave gratuita en https://aistudio.google.com/apikey
2. En la app, ve a **Progreso → Datos y ajustes → Ajustes de IA**.
3. Pega la clave, toca **Probar la conexión** y después **Guardar**.

La clave se guarda solo en ese móvil. **No la pongas nunca en los archivos del repositorio**, porque es público.

## Cosas importantes

- **Los datos viven en cada dispositivo.** Lo que apuntes en el móvil no aparece en el ordenador ni en la versión de Claude. Para pasar datos de uno a otro: **Guardar copia** en uno e **Importar copia** en el otro.
- **Haz copias de vez en cuando.** Si borras los datos del navegador o desinstalas la app, se pierden. La app te avisa si hace más de dos semanas que no guardas una copia.
- **Para actualizar la app**, sube el nuevo `index.html` con **Add file → Upload files** (sustituye al anterior). Sube también `sw.js` cuando venga en la actualización. Si algún día cambias los iconos a mano, sube el número de versión que hay al principio de `sw.js` (por ejemplo, de `pizarra-v2` a `pizarra-v3`).
