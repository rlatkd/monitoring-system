FROM    node:alpine as builder
WORKDIR /client
COPY    . /client
RUN     rm -rf node_modules/
RUN     npm install --force
RUN     chmod +x node_modules/.bin/vite
CMD     [ "npm", "run", "dev" ]
EXPOSE  3000