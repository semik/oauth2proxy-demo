# oauth2proxy-demo

Demonstration how to use OAuth2 Proxy in front of service.

## Apache with PHP behind OAuth2 Proxy

In directory [1-withPHPinApache](1-withPHPinApache) is example Docker Compose file which can help you exec demonstration. When you access http://localhost:4180/ which is port where OAuth2 Proxy is running you will first be asked to **Sign in with GitLab**:

![image](https://github.com/user-attachments/assets/92db9a39-3700-47c6-9f42-49ec8e013496)

later you can see JWT which was issued for your login session:

![image](https://github.com/user-attachments/assets/252ada17-b79c-4d58-ac22-83bb921f600c)

and also enviroment variables:

![Screenshot at 2024-09-27 12-05-55](https://github.com/user-attachments/assets/b0266f6a-75f8-4aac-848e-8785a28b3b1c)

To get this demo working you need to registrer your client in gitlab.com administrative interface and provide secrets values into `docker_secrets.env` see [docker_secrets.env.example](1-withPHPinApache/docker_secrets.env.example) for an example.
