FROM  node:20
RUN useradd expense
RUN mkdir /opt/server
ENV DB_HOST=mysql
RUN chown expense:expense -R /opt/server
WORKDIR  /opt/server
COPY package.json .
COPY *js .
RUN npm install
CMD [ "node" , "index.js" ]
