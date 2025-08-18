# # Use Nginx as the base image
# FROM nginx:alpine

# # Remove default Nginx HTML
# RUN rm -rf /usr/share/nginx/html/*

# # Copy all files from the current directory into Nginx's web directory
# COPY . /usr/share/nginx/html/

# # Ensure Nginx can read the files
# RUN chmod -R 755 /usr/share/nginx/html

# # Expose port 80 for web traffic
# EXPOSE 80

# # Start Nginx in the foreground
# CMD ["nginx", "-g", "daemon off;"]

FROM nginx:alpine

# Copy all HTML files to nginx html folder
COPY . /usr/share/nginx/html/

# Ensure nginx can read the files
RUN chown -R nginx:nginx /usr/share/nginx/html && chmod -R 755 /usr/share/nginx/html


