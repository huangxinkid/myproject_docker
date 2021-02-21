FROM nginx:latest
RUN rm /etc/nginx/conf.d/default.conf \
 && mkdir -p /usr/share/nginx/html/static \
 && mkdir -p /usr/share/nginx/html/media
ADD ./mysite_80.conf /etc/nginx/conf.d/
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]