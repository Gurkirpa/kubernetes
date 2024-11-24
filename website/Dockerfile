# Use the official Apache HTTP Server image as the base
FROM httpd:latest

# Copy the website content to the default directory served by httpd
COPY ./cafe-website/ /usr/local/apache2/htdocs/

# Ensure that the httpd service is enabled and restarted during runtime
# Note: This step is not required in the httpd container since it automatically runs httpd as its default entrypoint.

# Expose the default HTTP port
EXPOSE 80

# Restart the httpd service during container start (handled by CMD)
CMD ["httpd-foreground"]
