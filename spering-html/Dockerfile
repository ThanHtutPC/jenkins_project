FROM nginx

# Copy files to the nginx html directory
COPY . /usr/share/nginx/html/

# Expose the port nginx will run on
EXPOSE 80

# Start nginx
CMD ["nginx", "-g", "daemon off;"]
