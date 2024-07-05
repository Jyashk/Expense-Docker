FROM node:20-alpine
ENV DB_HOST=mysql
RUN useradd -D expense
RUN mkdir /app
WORKDIR /app
COPY  * /app
RUN npm install
EXPOSE 8080
USER expense
CMD [ "node", "index.js" ]