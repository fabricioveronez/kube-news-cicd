FROM cgr.dev/chainguard/node
WORKDIR /app
COPY --chown=node:node package*.json ./
RUN npm install
COPY --chown=node:node . . 
USER node
EXPOSE 8080
CMD ["node", "server.js"]
