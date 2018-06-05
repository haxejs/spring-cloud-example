FROM node:8-alpine
MAINTAINER Richard Shi

#alpine base image does not have git and gyp g++ toolchain
RUN apk add --no-cache git python binutils-gold curl g++ gcc gnupg libgcc linux-headers make

ADD .   /opt/cloud
RUN cd /opt/cloud && npm install && npm cache clean --force
WORKDIR /opt/cloud

# Start cloud
EXPOSE 3000
CMD ["node", "index.js"]
