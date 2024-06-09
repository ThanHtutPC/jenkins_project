FROM nginx

# Copy files to the nginx html directory
COPY /home/thanhtut/testing_project/jenkins_project/spering-html/ /usr/share/nginx/html/

# Expose the port nginx will run on
EXPOSE 80

# Start nginx
CMD ["nginx", "-g", "daemon off;"]
