#Base Images
FROM node
#Maintenair contact
LABEL MAINTAINER osler.santi@gmail.com
#Clone the project codes
RUN git clone -q https://github.com/docker-in-practice/todo.git
#cd to the directory to and make it startup directory
WORKDIR todo
#Install the dependencies
RUN npm install > /dev/null
#Expose the port 8000
EXPOSE 8000
#startup command
CMD ["npm", "start"]

