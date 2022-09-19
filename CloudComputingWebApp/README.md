Simple Web Chat Application with Chatbot using Microservices.

Main_code zip file has the complete Web App code and is deployed to Azure Web App and also to Azure VM.
Functionality: It has complete front-end and back-end code with APIs that calls the microservice which are deployed to different services like Heroku.

Heroku_Microservice zip file has code that is deployed to Heroku Web App.
Functionality: API from our Web Application (Azure App service) calls this Heroku microservice to give the user his Age, Chinese zodiac name or LCM and HCF based on the user's preference. 

Auth_MongoDB zip file the code that is deployed to other Heroku Web App.
Functionality: API from our Web Application (Azure App Service) calls this Heroku microservice to register the user and store the data in MongoDB. It also authenticates the users to login to chat window.

Below image repsresents architectural view of our entire web application.
![image](https://user-images.githubusercontent.com/36757754/191117922-13207837-555a-4a61-be96-cab9c173b5bf.png)
Implemented this project in form of sprints in total of 3 sprints.

Sprint 1:
