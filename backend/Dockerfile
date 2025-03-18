#FROM node:20
WORKDIR /opt/backend
COPY package.json ./
COPY *.js ./
RUN npm install
ENV DB_HOST="mysql"
WORKDIR /opt/backend
COPY --from=builder /opt/backend /opt/backend
CMD ["node", "index.js"]