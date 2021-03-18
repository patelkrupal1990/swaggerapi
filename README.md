# Implementation of Swagger API using postman
Swagger API testing using postman for petstore and user.

1. Ensure that you have Node.js >= v10 (https://nodejs.org/en/download/package-manager/)
2. Clone the repo https://github.com/patelkrupal1990/swaggerapi.git
3. Go to the cloned repo
4. Run npm install
5. Run npm run test:petstoreapi
6. Run npm run test:userapi

A directory with newman will be created having the report associated to it.Attached is the screenshot of the report of the api run.

https://github.com/patelkrupal1990/swaggerapi/blob/main/report.png


# Jenkins configuration

1. Create a job in jenkins.
2. Configure a job and add new execute shell.
3. Add below commands in the execute shell
    
    npm run test:petstoreapi
    
    npm run test:userapi
4. Trigger the job and you will see the API running in the console and html report generated in the newman folder.
5. Make sure you add the newman folder in the build artifact to preserve the reports for later use.


