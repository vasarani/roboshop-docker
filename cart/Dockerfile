FROM node:20
# this creates /app and move there
WORKDIR /app
COPY package.json .
COPY *.js .
ENV REDIS_HOST="true" \
    CATALOGUE_HOST="catalogue" \
    CATALOGUE_PORT="8080"
EXPOSE 8080
RUN npm install
CMD ["node", "server.js"]