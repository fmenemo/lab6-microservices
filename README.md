1.  
 1. Two microservices running: ![Microservices](/images/Microservices_Running.png)
 2. Two microservices running with additional info: ![Microservices with more info](/images/Microservices_more_info.png)
 3. Logs: ![Logs](/images/terminal1.png)
2. Service registration service: ![Service registrarion service](/images/Service_status.png)
3.  
 1. Additional account microservice: ![Additional account microservice](/images/New_microservice.png)
 2. Service registrarion with new microservice: ![Service registrarion with new microservice](/images/Service_status_another_service.png)
 3. Logs: ![Logs](/images/terminal2.png)
4. Service status after killing accounts in 2222: ![New service status](/images/Keeps_working.png)

After a brief downtime, the service keeps working. This happens because the system is correctly set up and therefore the web server configuration is searching for an application that is registered in the service with the name: ACCOUNTS-SERVICE. Since the new account microservice in port 4444 is registered with that name, it can recieve petitions from the web microservice.
