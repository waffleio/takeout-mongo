takeout-mongo
=============

This is the Docker container for housing mongodb

### Why?
* Because sometimes the official mongo image ends up broke, preventing new
  takeout signups from completing a successful installation
* This is a buffer to ensure we always have a working version of mongo available
  to our users

### How
* Browse to our [fork of the official mongo docker
  image](https://github.com/waffleio/mongo)
* Make the neccessary modifications to the specific version we desire
* push that built image to `quay.io/waffleio/official-mongo:<TAG>`
* modify the Dockerfile in THIS repo, update as necessary
