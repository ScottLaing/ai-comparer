<h2>ai-comparer</h2>

a side project to compare ai generation results (gemini, chatgpt) in a web app

very early stages, under construction/wip, check back soon

<h3>Misc Setup Steps</h3>

<h4>build and run locally</h4>

(install nodejs if not installed) <br/>
install node via web download if on windows, or on mac or linux as per those environments

(install yarn if not installed) <br/>
**npm install -g yarn**

(install app) <br/>
**yarn install**

(run app) <br/>
**node src/index.js**

(To view the web app in a browser) <br/>
in your browser run: <br/>
**http://localhost:3000/**

<h4>build docker image</h4>

(To build the docker image) <br/>
**docker build -t ai-comparer .**

(To run the docker container) <br/>
**docker run -dp 127.0.0.1:3000:3000 ai-comparer** 

(To run the web app in a browser)
in your browser run: <br/>
**http://localhost:3000/**

<h4>stop the running docker container</h4>

1) in Windows you can use docker desktop app to start/stop/delete containers

2) in git bash on windows (or linux or mac) you can use:

   a) get running container id via this command (or similar)
   
   **docker ps | grep ai-comparer | awk '{print substr($0, 0, 10)}'**

   b) stop this container

   **docker stop <container_id>**





