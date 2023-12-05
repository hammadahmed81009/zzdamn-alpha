FROM nginx:alpine

# Copy the static content into the Nginx server
COPY ./ /usr/share/nginx/html/

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
