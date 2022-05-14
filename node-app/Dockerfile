FROM node:16-alpine
WORKDIR /app
# to create build image working directory to avoid replace of file if we use root directory for image build
COPY package.json .
RUN npm install

COPY . .
# copy from current directory

# use during build time can be more than one
EXPOSE 5000
CMD [ "npm", "run", "dev" ] 
# to start application at the very end


