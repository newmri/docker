FROM node

WORKDIR /app

COPY package.json .

RUN npm install -g pnpm && pnpm install

COPY . .

EXPOSE 80

ENV MONGODB_USERNAME=root
ENV MONGODB_PASSWORD=secret

CMD ["pnpm", "start"]