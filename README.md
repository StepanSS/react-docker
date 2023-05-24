## React in Docker

### Install React

```bash
npm install -g create-react-app@3.4.1
```

### Generate a new app:
```bash
npm init react-app sample --use-npm
cd sample
```

### Build the image and fire up the container:
```bash
# debug mode
docker-compose -f ./docker/docker-compose.yml up -d --build
docker-compose -f ./docker/docker-compose.yml stop

# production mode
docker-compose -f ./docker/docker-compose.prod.yml up -d --build

```