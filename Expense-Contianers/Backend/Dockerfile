FROM node:20
ENV DB_HOST=mysql
RUN useradd expense
RUN mkdir /app
WORKDIR /app
COPY  *.js /app
RUN npm install
EXPOSE 8080
USER expense
CMD [ "node", "index.js" ]