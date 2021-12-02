FROM nginx:stable-alpine

RUN rm -f /etc/nginx/conf.d/default.conf

COPY docker/nginx/configs/app.conf /etc/nginx/conf.d/app.conf

EXPOSE 80
