FROM node:12.5
WORKDIR /app
EXPOSE 4001
ADD package.json /app
RUN npm install --save-exact
COPY . /app
CMD ["npm", "start"]

