FROM nginx:alpine

COPY index1.html /usr/share/nginx/html/index1.html
COPY nginx.conf /etc/nginx/nginx.conf

EXPOSE 80

HEALTHCHECK --interval=30s --timeout=10s --retries=3 CMD curl -f http://localhost:80 || exit 1

CMD ["nginx", "-g", "daemon off;"]
