🎮 juego de Dibujo en Tiempo Real 🖼️

¡Bienvenido al Juego de Dibujo en Tiempo Real! Un desafío donde la creatividad y la rapidez se combinan para crear dibujos que se transmiten y sincronizan al instante entre jugadores. La aplicación está construida utilizando **React** en el cliente y **Node.js con Express y WebSockets** en el servidor.

---

## 🚀 ¿CÓMO FUNCIONA EL JUEGO?

El juego se divide en dos partes fundamentales:

### 1. Cliente (Aplicación React)
El cliente es la interfaz donde los jugadores interactúan:

- Dibuja en un lienzo: Los jugadores pueden crear dibujos que se sincronizan en tiempo real con los demás.
- Chat en tiempo real: Los jugadores pueden enviarse mensajes durante el juego.
- Interacción y sincronización: Las acciones se actualizan y sincronizan al instante utilizando WebSockets con Socket.io.

### 2. Servidor (Node.js + Express + WebSockets)
El servidor se encarga de toda la lógica del juego:

- Gestión de Conexiones WebSocket**: El servidor mantiene las conexiones entre jugadores y distribuye las actualizaciones del juego.
- Gestión de Partidas y Chat**: Controla el estado del juego y maneja los mensajes entre jugadores.
- Persistencia (Opcional)**: Se puede agregar una base de datos para almacenar resultados de partidas o dibujos.

---

## 🛠️ TECNOLOGÍAS UTILIZADAS

- Frontend: React
- Backend: Node.js + Express
- Comunicaciones en Tiempo Real: Socket.io
- Gestión de Conexiones WebSocket: WebSockets

---

## 🔧 CÓMO INTERACTÚAN EL CLIENTE Y EL SERVIDOR

### 1. Conexión WebSocket

- Socket.io permite que el cliente se conecte al servidor de manera bidireccional en tiempo real.
- Cuando un jugador dibuja algo, las coordenadas de los puntos se envían al servidor, que distribuye esa información a los demás jugadores para que vean los cambios en sus propios lienzos.
- El servidor también puede enviar mensajes al cliente, como actualizaciones de estado del juego o mensajes de chat.

### 2. Dibujo en el Lienzo

- Los datos de los dibujos (por ejemplo, coordenadas) se envían al servidor a través de WebSockets.
- El servidor luego distribuye esos datos a todos los demás jugadores, asegurando que todos vean los mismos cambios en tiempo real.

### 3. Chat en Tiempo Real

- Los jugadores pueden enviar mensajes en el chat, los cuales son transmitidos por el servidor a todos los jugadores conectados.

### 4. Interactividad y Sincronización

- Las acciones de los jugadores (dibujos, mensajes, etc.) se sincronizan instantáneamente para que todos vean la misma información en tiempo real.

---

## 🏁 PASOS PARA JUGAR

### 1. Iniciar el Servidor

En la carpeta `server`, ejecuta:

```bash
npm start

### 2. iniciar el juego
En la carpeta `client`, ejecuta:
```bash
npm start


