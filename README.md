# ISLAS

Juego de mesa online para 3–5 jugadores: pueblos, recursos, barcos y volcanes.
Cada jugador juega desde su casa; las plazas libres las ocupan bots.

## Cómo jugar

1. Abre la página del juego (`index.html`).
2. Escribe tu nombre y pulsa **Crear mesa**. Aparece un código de 4 letras.
3. Tus amigos abren la misma página, escriben su nombre y entran con ese código
   (o pulsando la mesa en la lista de mesas abiertas).
4. El anfitrión elige el número de jugadores (3–5) y pulsa **Empezar partida**.

Mientras dura la partida, el anfitrión debe mantener la página abierta: es quien lleva el estado.
Si la recarga, la partida continúa donde estaba.

Si te equivocas, **Deshacer** anula tus jugadas del turno en curso (salvo después de mirar cartas
con Brujería), y **Cambiar elección** te deja cambiar de personaje hasta que elija el último jugador.

También se puede jugar en solitario contra bots, sin conexión.

El juego está en **español e inglés**: el selector ES / EN de la parte superior cambia el idioma al
momento y lo recuerda para la próxima vez. Cada jugador elige el suyo; en una misma partida unos pueden
jugar en español y otros en inglés.

## Publicar en GitHub Pages

1. Sube `index.html` (y este README) al repositorio.
2. En el repositorio: **Settings → Pages → Deploy from a branch**, rama `main`, carpeta `/ (root)`.
3. El juego quedará en `https://<tu-usuario>.github.io/<repositorio>/`.

## Conexión online

Fuera de claude.ai la conexión usa **Supabase Realtime** (solo canales en tiempo real; no crea tablas
ni guarda datos). La URL del proyecto y la clave pública están en el objeto `SUPA` dentro de
`index.html`. La clave publicable está pensada para ir en páginas web públicas.

Para ver los mensajes de conexión en la consola del navegador, añade `?debug=1` a la dirección.

Dentro de claude.ai el juego usa las salas de Claude, que solo admiten a personas con acceso compartido
a la página. Para jugar con cualquiera, usad todos el enlace de GitHub Pages.

## Reglamento

Basado en *ISLAS · Reglamento de prototipo*. Los puntos que el reglamento deja abiertos están
resueltos en la sección «Reglas rápidas y decisiones del prototipo» de la propia página.
