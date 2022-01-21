# busca ultima tag da imagem do node
FROM node:current-alpine3.15
# define o diretorio de trabalho
WORKDIR /app
# copia os arquivos package*json para instalacao das libs
COPY package*.json ./
# realiza a instalacao das libs
RUN npm install
# copia o restante dos arquivos
COPY . .
# expor a porta
EXPOSE 8080
# executa o sistema
ENTRYPOINT ["node", "server.js"]