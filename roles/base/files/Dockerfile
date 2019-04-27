FROM node:10 AS dependencies
ADD package.json .
RUN npm install

FROM dependencies
ADD index.mjs .
ADD config.mjs .
ADD auth.mjs .
ADD passport.mjs .
ADD auth.mjs .
ADD rest rest
EXPOSE 3000
ENTRYPOINT [ "node", "--experimental-modules", "index.mjs" ]