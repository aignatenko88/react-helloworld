FROM nginx:stable-alpine

RUN \
	rm -f /etc/nginx/conf.d/default.conf \
	&& mkdir -p /etc/nginx/ssl

COPY docker/nginx/configs/demo.github.actions+3-key.pem /etc/nginx/ssl/demo.github.actions+3-key.pem
COPY docker/nginx/configs/demo.github.actions+3.pem /etc/nginx/ssl/demo.github.actions+3.pem
COPY docker/nginx/configs/app.conf /etc/nginx/conf.d/app.conf

EXPOSE 443
