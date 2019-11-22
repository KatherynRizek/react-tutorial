# react-tutorial
Start with an empty project directory

## Add node with docker
* Create a `Dockerfile` and paste the contents of `react-tutorial/Dockerfile`
* Create a `startup.sh` file and paste the contents of `react-tutorial/startup.sh`
* Run the command `docker build . -t create-react-app` to build your container
* Create a `tutorial` directory at the same level as your `Dockerfile`. Tutorial can be replaced with whatever you would like to name the app.
* You should still be at the highest level of your project directory (the same level as the `Dockerfile`). Run the command `docker run -v $PWD:/project create-react-app tutorial`. Tutorial should be replaced with whatever you named your app. This command is for linux, it may differ on a different OS. For windows in git bash, use: `docker run -v /$(pwd):/project create-react-app tutorial`

## Add react with docker
* Move into your `tutorial` directory
* Create a `Dockerfile` and paste the contents of `react-tutorial/tutorial/Dockerfile` 
* Create a `docker-compose.yml` and paste the contents of`react-tutorial/tutorial/docker-compose.yml`
* Run `docker-compose up -d` to build the container
* To stop the container, run `docker-compose stop`
