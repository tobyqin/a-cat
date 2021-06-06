# A Cat App

Nodejs demo app to run with Docker. This app displays a random picture of a cat.

## Build and run locally

You should have nodejs 12+ & npm 5+ installed locally.

```bash
npm install
node app.js
```

Open [http://localhost:3000/](http://localhost:3000/) in your web browser to
view the running app.

## Build and run with Docker

```bash
# build Dockerfile, please change username in the command
docker build -t tobyqin/a-cat:latest .

# run it
docker run -it --rm -p 3000:3000 tobyqin/a-cat

# publish to docker hub
docker login
docker push tobyqin/a-cat
```

## Just use it

This cat app has already been published to docker hub, you can run it by:

```bash
docker run -d -p 3000:3000 --restart=always tobyqin/a-cat
```
