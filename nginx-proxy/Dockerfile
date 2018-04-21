FROM nginx as base

RUN apt-get update && \
    apt-get install -y curl

RUN rm -r /etc/nginx 
COPY nginx /etc/nginx 
COPY index.html 50x.html /usr/share/nginx/html/

CMD ["nginx-debug", "-g", "daemon off;"]


