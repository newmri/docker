FROM node

WORKDIR /app

COPY package.json .

RUN npm install -g pnpm && pnpm install

COPY . .

EXPOSE 3000

ENV NODE_OPTIONS=--openssl-legacy-provider

CMD ["pnpm", "start"]