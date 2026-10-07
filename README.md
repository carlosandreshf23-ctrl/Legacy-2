# Legado: Perú — Pisco, septiembre de 1820

Juego de exploración en pixel art ambientado en Pisco durante la llegada de la
Expedición Libertadora. Todo el juego está en un solo archivo HTML.

## Cómo jugar

Abre `juego/LegadoPeru-Pisco1820.html` en Chrome o Edge (con internet).
Las instrucciones para jugar con amigos están en `juego/LEEME.txt`.

## Estado

- Multijugador por código de sala (P2P): chat, gestos y regalos entre jugadores.
- **Todo en vivo con el anfitrión:** quien crea la sala manda sobre los vecinos,
  los animales, la hora, el clima, las casas, el fuego y los eventos (sismos,
  tsunami, huaico, carreta, procesión de las ánimas).
- **Lo que hace cada jugador llega a todos:** golpear o matar vecinos, romper,
  mover, prender o llevarse objetos, derribar tramos de muro, prender fuego y
  apagarlo con agua.
- **Sin lag:** el anfitrión manda 10 veces por segundo solo lo que cambió (foto
  completa cada segundo); cada envío cuesta ~0,1 ms y, con todo el pueblo en
  movimiento, unos 30 KB/s. Los invitados mueven a cada vecino y animal con
  suavizado, sin saltos.

## Límites conocidos

- Los vecinos que pelean o persiguen siguen al anfitrión; si un invitado los
  golpea, huyen en lugar de atacarlo.
- Los animales que un invitado carga o monta solo se mueven en su pantalla.
- Los misterios personales (la sombra del camino viejo, etc.) siguen siendo de
  cada jugador.
- Todo esto funciona con la sala con código; la sala de claude.ai solo comparte
  día, hora, muertos y casas caídas.
