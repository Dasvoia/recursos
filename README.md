# Biblioteca de recursos — Dasvo IA Builders

**En vivo:** https://dasvo-recursos.vercel.app

La página pública donde la comunidad descarga todo lo de cada video.

Es una sola página HTML sin dependencias. Se abre con doble clic en cualquier
computador y funciona igual publicada en internet.

```
index.html          la página
descargas/          todo lo que la gente descarga
```

---

## Cómo agregar un video nuevo

Es lo único que vas a tener que hacer de aquí en adelante. Toma 5 minutos.

1. Mete los archivos nuevos en `descargas/`.
2. Abre `index.html` y busca esta línea:

```
<!-- ====== AQUI SE AGREGAN LOS VIDEOS NUEVOS ======
```

3. Copia el bloque completo que empieza en `<article class="video">` y termina
   en `</article>`, pégalo justo debajo de ese comentario, y cámbiale:
   - el número dentro de `<span class="badge">VIDEO 1</span>`
   - el título `<h3>` y la descripción `<p>` del encabezado
   - las líneas `<a class="rec">` por los recursos de ese video

4. Sube el cambio. La página se actualiza sola.

Lo más nuevo va **al final** de la lista, como está anunciado en la portada.

### Si prefieres no tocar el HTML

Pégale esto a Claude Code parado en esta carpeta:

```
En index.html, agrega un video nuevo a la biblioteca. Copia el bloque
<article class="video"> que ya existe, pégalo justo debajo del comentario que
dice "AQUI SE AGREGAN LOS VIDEOS NUEVOS", y cámbiale el número, el título, la
descripción y los recursos. Te los paso ahora. Respeta el estilo exacto de las
líneas que ya están.
```

---

## Los colores de los puntitos

Cada recurso tiene un punto de color que dice de qué tipo es:

| Clase | Color | Para qué |
|---|---|---|
| `punto` | verde | Empieza aquí, lo primero que debe abrir |
| `punto pdf` | azul | Guías en PDF |
| `punto tool` | morado | Plantillas, gráficos y herramientas para abrir |
| `punto zip` | ámbar | Paquetes completos |

---

## Publicar

Está pensada para Vercel: se conecta este repositorio y queda publicada sola.
Cada vez que subas un cambio, Vercel republica en unos segundos.

También funciona en GitHub Pages sin cambiar nada.
