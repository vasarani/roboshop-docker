FROM node:20
# this creates /app and move there
WORKDIR /app1
ENV REDIS_HOST="true" \
    CATALOGUE_HOST="catalogue" \
    CATALOGUE_PORT="8080"
EXPOSE 8080
COPY package.json .
COPY *.js .
RUN npm install
CMD ["node", "server.js"]