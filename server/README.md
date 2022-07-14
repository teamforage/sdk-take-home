# Payment Server

## Setup

Make sure you've installed docker. I suggest you install Docker Desktop.
  - [Mac](https://docs.docker.com/desktop/install/mac-install/)
  - [Windows](https://docs.docker.com/desktop/install/windows-install/)
  - [Linux](https://docs.docker.com/desktop/install/linux-install/)


### Option a: docker compose

1. Run Docker Desktop or docker engine
1. Make sure you have [docker compose installed](https://docs.docker.com/compose/install/)
1. From within this directory (`cd ./server`), run the following command to spin up the server: `docker compose up`
1. This commmand will spin up one container: `dev_server_api` is the development server. It will validate your requests, yield errors, and yield random successful request bodies. You can access it through `http://0.0.0.0:8080/`

Here's an example of what you should see:
![CleanShot 2022-07-13 at 17 30 31@2x](https://user-images.githubusercontent.com/10040882/178859577-130571f3-84ad-4b24-86eb-6d9b6812952b.png)


### Option b: docker

1. Run Docker Desktop or docker engine
1. Make sure you have docker installed
1. Run the docker container: `docker run -v $PWD/oas.yml:/app/oas.yml -p 8080:808 stoplight/prism mock -h 0.0.0.0 -p 8080 -d /app/oas.yml`
1. The server will run on `http://0.0.0.0:8080/`

Here's an example of what you should see:
![CleanShot 2022-07-13 at 17 42 46@2x](https://user-images.githubusercontent.com/10040882/178860600-9a011e3f-edaa-4a43-afc4-f3d08750f6b6.png)
