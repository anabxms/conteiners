# CONTEINER - Frontend Angular: frontend 

Para o App Angular, utilizamos o seguinte DockerFile:

```
FROM nginx:alpine
COPY ./dist/app-angular/ /usr/share/nginx/html/
RUN npm install
CMD ng serve
```

Criar a imagem:  `docker build -t frontend .`

Com isso, se rodarmos “ docker images” a imagem deve aparecer. 

Para executar: `docker run -it --rm -p 9000:80 frontend`