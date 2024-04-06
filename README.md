O "Web server 1" (web-server-node-internal-http-module.js) só precisa do Node instalado, pois só usa o módulo HTTP, que é um módulo INTERNO dele, então ele roda mesmo fora da pasta dele, desde que o Node já esteja instalado no ambiente.

Já o "Web server 2" (web-server-node-express.js) só roda dentro da pasta dele, pois ele precisa do Express instalado no Node, pois usa o módulo EXPRESS.

Então somente foi necessário criar um arquivo package.json básico com a dependência Express e o valor "express": "^4.19.1" e depois rodar npm install dentro da pasta.
