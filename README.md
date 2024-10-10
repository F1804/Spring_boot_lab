# Spring_boot_lab
Demo for Spring Boot 
Simple REST Service
This project is a basic Spring Boot application that exposes a RESTful web service. The web service returns a greeting message, which can be customized with a name parameter.
Features
•	Spring Boot-based RESTful web service.
•	Returns a greeting message.
•	Customizable greeting by passing a name parameter.
•	Built with Maven and Java 11.
Tools and Technologies Used
•	Java (Version 11 or above)
•	Spring Boot (Version 2.7.0 or the latest stable version)
•	Maven for project dependency management
•	Postman (or any other REST client) for testing the endpoints
Getting Started
Prerequisites
To build and run the application, you will need:
•	Java 11 or higher installed on your machine.
•	An IDE like IntelliJ IDEA or Eclipse.
•	Maven installed (if not using an IDE with built-in Maven support).
•	Postman or any REST client to test the application.
Project Setup
1.	Project Initialization:
o	Go to Spring Initializr.
o	Set the following configurations:
	Project: Maven Project
	Language: Java
	Spring Boot: 2.7.0 or latest
	Group: com.example
	Artifact: simple-rest-service
	Name: SimpleRestService
	Package name: com.example.simplerestservice
	Packaging: Jar
	Java: 11
o	Add Dependencies: Spring Web
o	Click "Generate" to download the project and unzip it.
2.	Import the Project:
o	Open your IDE (IntelliJ IDEA, Eclipse, etc.).
o	Import the unzipped project as a Maven project.
Running the Application
1.	Run the Application:
o	Open the SimpleRestServiceApplication class located in the src/main/java/com/example/simplerestservice package.
o	Right-click on the class and select Run SimpleRestServiceApplication.
o	The application will start on the default port 8080.
2.	Testing the Application:
o	Open Postman (or any other REST client).
o	Make a GET request to: http://localhost:8080/greeting
o	You should receive a response similar to: {
o	  "id": 1,
o	  "content": "Hello, World!"
o	}
o	Test with a custom name by making a GET request to: http://localhost:8080/greeting?name=John
o	The response will look like: {
o	  "id": 2,
o	  "content": "Hello, John!"
o	}
3.	Project Structure:
src/
 └── main/
     └── java/
         └── com/
             └── example/
                 └── simplerestservice/
                     ├── model/
                     │   └── Greeting.java
                     ├── controller/
                     │   └── GreetingController.java
                     └── SimpleRestServiceApplication.java
REST Endpoints
•	GET /greeting: Returns a default greeting message (Hello, World!).
•	GET /greeting?name=your_name: Returns a customized greeting message (Hello, your_name!).


![image](https://github.com/user-attachments/assets/4b4bd5aa-e07a-4de8-b14d-df17444761e5)
