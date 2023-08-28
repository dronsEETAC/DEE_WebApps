# WebApps
## 1. General description
The modules in this block are front-end desktop modules in the form of WebApps, developed using Vue and Ionic.   
WebApps are more accessible than Desktop applications. You do not need to install anything in your computer or mobile device. You only need a browser and internet connection. Using these WebApps, visitors to the DronLab will be able to interact easily with our drones using their mobile devices.    
Each of the modules in this block has a GitHub repo where you can find the code together with a description, installation instructions and demos. These are the repos:
* *DashApp*:
[![DroneEngineeringEcosystem Badge](https://img.shields.io/badge/DEE-DashApp-brightgreen.svg)](https://github.com/dronsEETAC/DashboardVueDEE) allows the global control of the system (arm, take-off and guide the drone, define flight plans, process data coming from the drone, etc.).
   
* *Mobile app*:
[![DroneEngineeringEcosystem Badge](https://img.shields.io/badge/DEE-MobileApp-brightgreen.svg)](https://github.com/dronsEETAC/IonicVueMobileAppDEE) a WebApp with a reduced set of functionalities that can be operated from a mobile phone or Tablet connected to internet.

* *Dashboard Games*:
[![DroneEngineeringEcosystem Badge](https://img.shields.io/badge/DEE-DashboardGames-brightgreen.svg)](https://github.com/dronsEETAC/DashboardGames) a WebApp to control a variety of games, including Drone Circus, a Controllers Game and Follow Me Game.

* *Mobile Web App*:
[![DroneEngineeringEcosystem Badge](https://img.shields.io/badge/DEE-MobileWebApp-brightgreen.svg)](https://github.com/dronsEETAC/MobileWebApp) a WebApp to allow visitors to play the games (controlled by Dashborar Games) using their own mobile phones.

## 2. Node, Vue and Ionic
In order to run and contribute to the modules in this block, you need to install Node.js (version v16.14.2) and @vue/cli version 4.5.15 and @ionic/cli (in case of the Mobile app). We recommend Visual Code as IDE for development in Vue.
## 3. Secure WebApps
Some of the WebApps require access to sensible data in the mobile device (location, microphone, camera). This requires secure (https) access to the WebApps. See the tutorial referred bellow to learn how to implement secure WebApps.
## 4. Frequent error
When running the code you may get errors such as this:

Module not found: Error: Can't resolve 'fs' in 'C:\Users\USER\Documents\Miguel\DEE_all_repos\IonicVueMobileAppDEE\node_modules\opencv.js'

In this case, you must include the following code in the package.json in node-modules/opencv.js:     
```
  "browser": {
    "fs": false,
    "path": false,
    "os": false,
    "crypto": false
  }
  ```
## 5. Serving the WebApps in production
The WebApps in this block are currently being served in a server in the Campus, according to the following table:

## 6. Supporting materials   
A tutorial (in Spanish) on Vue, also focused in how to develop web app for the ecosystem:      
[Vue for the ecosystem](https://www.youtube.com/watch?v=XCn9stPZ4iY&list=PL64O0POFYjHoeq8dfP-XYPCoNlehSiR_B)
     
A tutorial (in Spanish) on Vue + Ionic, also focused in how to develop mobile web app for the ecosystem:      
[Vue + Ionic for the ecosystem](https://www.youtube.com/playlist?list=PLT01gtFyuSL5MKxNFBtEkah45xEJqqCCn)

A tutorial (in Spanish) on how to implement secure WebApps:
[Secure WebApps for the ecosystem](https://www.youtube.com/playlist?list=PLyAtSQhMsD4qbgXn6jheozHsjU4GRCqtv)
