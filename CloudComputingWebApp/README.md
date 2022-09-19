**Simple Web Chat Application with Chatbot using Microservices:**

**Main_code** zip file has the complete Web App code and is deployed to Azure Web App and also to Azure VM.
Functionality: It has complete front-end and back-end code with APIs that calls the microservice which are deployed to different services like Heroku.

**Heroku_Microservice** zip file has code that is deployed to Heroku Web App.
Functionality: API from our Web Application (Azure App service) calls this Heroku microservice to give the user his Age, Chinese zodiac name or LCM and HCF based on the user's preference. 

**Auth_MongoDB** zip file the code that is deployed to other Heroku Web App.
Functionality: API from our Web Application (Azure App Service) calls this Heroku microservice to register the user and store the data in MongoDB. It also authenticates the users to login to chat window.

Below image repsresents architectural view of our entire web application.
![image](https://user-images.githubusercontent.com/36757754/191117922-13207837-555a-4a61-be96-cab9c173b5bf.png)
Implemented this project in form of sprints in total of 3 sprints.

**Sprint 1:**
This project features usage of Google Cloud Shell (local machine), BitBucket (repository), Azure App Service (cloud service for one microservice) and Heroku (cloud
service for the other microservice).
Microservice1 is designed to get the year and generate Age and Leap year check.
Microservice2 is designed to provide the LCM and HCF for any two given input numbers.
The code for the main Web Application resides in the public BitBucket repository. This web application has 2 microservices each hosted on Azure and Heroku respectively.
Azure App Service has been linked with a private bitbucket repository to get the code for the microservice1.
Heroku has been linked with another private bitbucket repository to get the code for the microservice2.
![image](https://user-images.githubusercontent.com/36757754/191129928-0f16f214-37ca-415e-9eaa-cfc9a1f30d4a.png)

**Sprint 2:**
Coded the website to store registration credentials of users in MongoDB database and also use this data to validate the user when the user tries to login to the web application. Display connected users list, enabled private chats with each user and also retrieve the chat history from MongoDB database.
![image](https://user-images.githubusercontent.com/36757754/191130198-082acb15-a08a-4e89-bd83-836335a6db3f.png)

**Sprint 3:**

