# specify a parent image (node17 and linnux alpine)
FROM node:17-alpine

# specify a working directoory of image
WORKDIR /app

# copy all the sources files
COPY . .

# RUn the npm instaall at build time to add all the dependencies to the image
RUN npm install

# expose the working Port
EXPOSE 4000

# command run only whe container of this iage is run
CMD [ "node", "app.js" ]

# to build image container
# t is to add tag
#  the  . is a relative path for the image
# docker build -t nameTag .