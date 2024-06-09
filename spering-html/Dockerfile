FROM nginx

# Create a non-root user and group
RUN addgroup -S myusergroup && adduser -S myuser -G myusergroup

# Copy files to the nginx html directory
COPY /home/thanhtut/testing_project/jenkins_project/spering-html/ /usr/share/nginx/html/

# Change ownership of the files to the non-root user
RUN chown -R myuser:myusergroup /usr/share/nginx/html

# Switch to the non-root user
USER myuser

# Expose the port nginx will run on
EXPOSE 80

# Start nginx
CMD ["nginx", "-g", "daemon off;"]
