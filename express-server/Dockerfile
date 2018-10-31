FROM node

RUN mkdir -p /var/www/html

WORKDIR /var/www/html

COPY package.json /var/www/html

RUN npm install

COPY . /var/www/html

EXPOSE 3000

CMD  mongorestore /express-server/dump

CMD ["npm", "start"]