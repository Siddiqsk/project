# # Use Nginx as the base image
# FROM nginx:alpine

# # # Remove default Nginx HTML
# # RUN rm -rf /usr/share/nginx/html/*

# # Copy all files from the current directory into Nginx's web directory
# COPY . /usr/share/nginx/html/

# # # Ensure Nginx can read the files
# # RUN chmod -R 755 /usr/share/nginx/html

# # # Expose port 80 for web traffic
# # EXPOSE 80

# # # Start Nginx in the foreground
# # CMD ["nginx", "-g", "daemon off;"]

# Use lightweight Nginx base
FROM nginx:alpine

# Remove default Nginx HTML (optional)
RUN rm -rf /usr/share/nginx/html/*

# Copy your frontend build files to Nginx web directory
COPY . /usr/share/nginx/html/

# Fix permissions so Nginx can read the files
RUN chmod -R 755 /usr/share/nginx/html

# Expose port 80
EXPOSE 80

# Start Nginx in foreground
CMD ["nginx", "-g", "daemon off;"]
