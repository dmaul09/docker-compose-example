FROM nginx 
COPY ./default.conf /etc/nginx/conf.d/default.conf
FROM node:alpine
WORKDIR '/app'
COPY ./package.json ./
RUN npm install 
COPY . . 
CMD ["npm", "run", "start"]