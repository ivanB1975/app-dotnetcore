# HOW TO deploy a sample dotnet application to the Swisscom Cloud Foundry  
    
    
### Create a User Provided service that points to the external RabbitMQ service

To create a user provided service in cloud foundry it is necessary to use the command format:

    cf create-user-provided-service my-db-mine -p '{"username":"admin","password":"pa55woRD"}'

where the credentials of the service are passed to the command as stringified json object.