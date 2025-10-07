Sample Java SpringBoot web app used to demo CI/CD using Azure DevOps and deploying to Azure App Service.

``

IMPORTANT NOTES :

``
---- create self hosted pool or use which are hosted b microsoft

--- create a new poool : create a linux vm 

-- wget http :// download link

-- create pat and authenticate > organisttion > user settings 

--configure and connect mypool

--server url : dev.azure.com/ramankhanna


--install maven and git on self hosted server

--- run ./run.sh to start listening

--imp note : select none in code coverage seeting in ci part

``in the release stage , while authorizing to your webapp go to advanced section > select the third option > publish webapp > select ur webapp 


imp note : while creating release : in the "arificat download" section , select the dropdown folder > drop > maven gradle > target > .jar file "


while creating a azure app svc : select runtime stack :
   java 17 tomcat 9

---- Due to changes in Azure API, please refer to the following change to the Release pipeline:

Runtime Stack : Tomcat 9.0 with Java 17

Startup command:

java -jar /home/site/wwwroot/gs-spring-boot-0.1.0.jar --server.port=80


``
