FROM node:16-slim
WORKDIR /uploader-app
COPY app/. .
RUN npm i
EXPOSE 3000
CMD [ "node", "server.js" ]