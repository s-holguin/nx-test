FROM node:lts-alpine
WORKDIR /app
COPY ./dist/apps/info-all .
# COPY ./package.json .
# COPY ./package-lock.json .

ENV PORT=3000
EXPOSE ${PORT}
RUN npm install --production
RUN npm install typescript
# dependencies that nestjs needs
# CMD ["nx", "serve", "info-all", "--production"]
CMD ["npm", "run", "start"]