#*This is defining base image
FROM node:17-alpine

#* Specify working directory of project
# yaha jake hamara project run hoga
WORKDIR /app


#* package.json files ko working directory mein llao
COPY ./package.json .

#* Run the command after copying package.json

RUN npm install

# copy the current directory wali cheeze into docker directory
COPY . .

EXPOSE 3000

# we are using this command to runour deployment server

CMD ["npm", "start"]