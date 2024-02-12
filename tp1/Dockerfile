FROM node:12

# RUN apt update
# RUN apt upgrade
# RUN apt install build-essential sudo git
# RUN curl -fsSL https://deb.nodesource.com/setup_19.x > node.sh
# RUN chmod +x node.sh
# RUN bash node.sh

WORKDIR /app

COPY package*.json ./

RUN npm install

COPY . .

ENV PORT=8080

EXPOSE 8080

CMD [ "npm", "start" ]
