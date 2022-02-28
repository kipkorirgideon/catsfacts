FROM node:14-alpine

WORKDIR /app

COPY .  /app/

RUN rm  -rf ./package-lock.json

RUN npm install

RUN npm run build

WORKDIR /app/build


EXPOSE 5001

ENTRYPOINT ["node"]

CMD ["./app.js"]
