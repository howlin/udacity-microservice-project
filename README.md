
# Udacity Project - Refactor Udagram App into Microservices and Deploy

The project is split into three parts:

1.  [The Simple Frontend](/udacity-c3-frontend) A basic Ionic client web application which consumes the RestAPI Backend.

2.  [The RestAPI Feed Backend](/udacity-c3-restapi-feed), a Node-Express feed microservice.

3.  [The RestAPI User Backend](/udacity-c3-restapi-user), a Node-Express user microservice.

  

## Getting Setup

### Installing project dependencies

Install [Ionic Cli](https://ionicframework.com/docs/installation/cli) and [Node/NPM](https://nodejs.org/en/download/)


### Configure Environment Variables 
Create ~/.profile and add the following

```bash
export POSTGRESS_USERNAME=<>;
export POSTGRESS_PASSWORD=<>;
export POSTGRESS_DATABASE=<>;
export POSTGRESS_HOST=<>;
export AWS_REGION=<>;
export AWS_PROFILE=<>;
export AWS_BUCKET=<>;
export JWT_SECRET=<>;
export ENV_VALUE=<>;
```
Run ``` source ~/.profile```

### Configure The Backend Endpoint

Ionic uses enviornment files located in `./src/enviornments/enviornment.*.ts` to load configuration variables at runtime. By default `environment.ts` is used for development and `enviornment.prod.ts` is used for produciton. The `apiHost` variable should be set to your server url either locally or in the cloud.

### NPM Dependancies 

This project uses NPM to manage software dependencies.  ``` cd ``` into ``/udacity-c3-frontend``,  ``/udacity-c3-restapi-feed`` and ``/udacity-c3-restapi-user`` and run 

```bash 
npm install 
```


### Configure The Backend Endpoint

Ionic uses enviornment files located in `./src/enviornments/enviornment.*.ts` to load configuration variables at runtime. By default `environment.ts` is used for development and `enviornment.prod.ts` is used for produciton. The `apiHost` variable should be set to your server url either locally or in the cloud.

  

***

### Running the Development Server

Ionic CLI provides an easy to use development server to run and autoreload the frontend. This allows you to make quick changes and see them in real time in your browser. To run the development server, open terminal and run:

  

```bash
ionic serve
```

  

### Building the Static Frontend Files

Ionic CLI can build the frontend into static HTML/CSS/JavaScript files. These files can be uploaded to a host to be consumed by users on the web. Build artifacts are located in `./www`. To build from source, open terminal and run:

```bash
ionic build
```

***
