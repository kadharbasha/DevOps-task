# 1. Grab the latest node image
FROM node:12.5
# 2. Set the working directory inside the container to /app
WORKDIR /app
# 3. Add the .env to the directory (We need those variables)
# ADD .env /app
# 4. Expose port defined in .env file
EXPOSE 4000
# 5. Add package.json to the directory
ADD package.json /app
# 6. Install dependencies
RUN npm install --save-exact
# 7. Copy the rest into directory
COPY . /app
# 8. Build the resources
#RUN npm run build
# 9. FFMPEG installation
#RUN apt update
#RUN apt install ffmpeg -y

# 9. Start the app inside the container
CMD ["npm", "start"]

# 10. To build docker image
# docker build -t howzb .
# 11. Tag the image
# docker tag howzb <username>/howzb:latest
# 12. Publish the image
# docker push <username>/howzb:latest
