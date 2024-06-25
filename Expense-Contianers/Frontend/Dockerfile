FROM nginx      
USER nginx
RUN sudo rm -rf /usr/share/nginx/html/index.html
RUN sudo rm -rf /etc/nginx/nginx.conf
RUN sudo rm -rf /etc/nginx/conf.d/default.conf
COPY code /usr/share/nginx/html/
COPY expense.conf /etc/nginx/nginx.conf
