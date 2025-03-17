FROM node:20
WORKDIR /opt/backend
COPY package.json .
COPY *.js .
#it will install dependencies
RUN npm install
ENV DB_HOST="mysql"
CMD ["node", "index.js"]