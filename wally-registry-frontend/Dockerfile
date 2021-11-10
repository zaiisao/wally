FROM node:14.15
WORKDIR /app
EXPOSE 8000
COPY . .
RUN npm install
ARG REACT_APP_WALLY_API_ENVIRONMENT=https://api.test.wally.run
RUN npm run build
CMD ["node", "build/server/server.js"]
