# react-tutorial
Start with an empty project directory

## Add node with docker
* Create a `Dockerfile` and paste the contents of `react-tutorial/Dockerfile`
* Create a `startup.sh` file and paste the contents of `react-tutorial/startup.sh`
* Run the command `docker build . -t create-react-app` to build your container
* Create a `tutorial` directory at the same level as your `Dockerfile`. Tutorial can be replaced with whatever you would like to name the app.
* Run the command `docker run -v $PWD:/project create-react-app tutorial`. Tutorial should be replaced with whatever you named your app. This command is for linux, it may differ on a different OS
