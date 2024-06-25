FROM nginx      
USER root
# Create the directories with appropriate permissions
RUN mkdir -p /var/cache/nginx/client_temp && \
    chown -R nginx:nginx /var/cache/nginx
USER nginx
COPY code /usr/share/nginx/html/
COPY expense.conf /etc/nginx/nginx.conf
