FROM node:14

WORKDIR /app

COPY package.json ./

RUN npm i -g pnpm
RUN pnpm fetch
RUN pnpm install

COPY . ./
RUN pnpm run build

EXPOSE 3000

CMD ["pnpm", "start:prod"]