FROM nginx:alpine
COPY ./dist/app-angular/ /usr/share/nginx/html/
RUN npm install
CMD ng serve
