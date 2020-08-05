FROM node:12.2.0-alpine

WORKDIR /
COPY ./ /

ENV PATH /node_modules/.bin:$PATH

#COPY package.json /app/package.json
RUN npm install
RUN apk add  --no-cache ffmpeg

CMD ["node", "ws-rtsp-server.js"]
