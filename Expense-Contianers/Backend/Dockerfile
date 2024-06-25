FROM node:20
ENV DB_HOST=mysql
RUN useradd expense
RUN mkdir /app
WORKDIR /app
ADD https://expense-builds.s3.us-east-1.amazonaws.com/expense-backend-v2.zip /app/
RUN unzip *.zip
RUN npm install
EXPOSE 8080
CMD [ "node", "index.js" ]