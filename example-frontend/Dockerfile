ARG NODE_VERSION=16.20.2
FROM node:${NODE_VERSION}

WORKDIR /myapp

COPY . .

RUN npm install


#ARG REACT_APP_BACKEND_URL=http://localhost:8080
RUN  npm run build

RUN npm install -g serve


CMD ["serve", "-s", "-l", "5000", "build"]