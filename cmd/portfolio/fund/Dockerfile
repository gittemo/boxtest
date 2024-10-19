# Use the official NGINX image as the base
FROM nginx:alpine

# Remove the default NGINX welcome page
RUN rm /usr/share/nginx/html/index.html

# Copy your custom index.html to the NGINX html directory
COPY index.html /usr/share/nginx/html/index.html

# Expose port 80 to allow external access
EXPOSE 80

# Start NGINX when the container launches
CMD ["nginx", "-g", "daemon off;"]