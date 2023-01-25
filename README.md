# ServidorNode.js
Mi primer servidor creado con Node.js.

//Mi primer servidor con el módulo HTTP.
const http = require('http');

const servidor = http.createServer((req, res) => {
  console.log("Solicitud nueva.");
  res.end('¡Hola mundo!');
});

const PUERTO = 3000;

servidor.listen(PUERTO, () => {
  console.log(`El servidor esta escuchando en el puerto http://localhost:${PUERTO}.`);
});
