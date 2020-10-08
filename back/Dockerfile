FROM node as builder

WORKDIR /app
COPY package.json /app/package.json
# RUN apt-get --no-cache add --virtual builds-deps build-base python
COPY . /app
RUN npm install

EXPOSE 9000
CMD ["npm", "start"]
