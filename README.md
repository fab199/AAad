`This Project Involves 3 steps which is: 1.Setup of The App stack 2.Containerization of microservice App and 3.Deployment of the microservice App on Kubernetes Cluster`

<h2>STEP 1: SETUP OF THE MICROSERVICE APP STACK(VPROFILE)</h2>

**Project Architecture**

<br/>
<img src="https://i.imgur.com/M3xRoer.png" height="80%" width="80%" alt="PROJECT ARCHITECTURE"/>
<br />
The architectural design outlined in the transcript describes the structure and interaction of various components within the V Profile Project Setup Local. Here's an explanation of the architectural design:

1. **User Interaction**:
   - Users interact with the web application by accessing it through a web browser. by using a domain name (URL)

2. **Load Balancing with Nginx**:
   - Nginx is employed as a web server and reverse proxy to manage incoming user requests and distribute them across multiple instances of the Tomcat server. It acts as a load balancer to evenly distribute traffic.

3. **Apache Tomcat**:
   - Apache Tomcat is utilized as a Java-based web application server to host the social networking web application. It handles requests from users and executes the application's logic.

4. **RabbitMQ**:
   - RabbitMQ is included in the architecture to introduce a level of complexity and practice for the learner. While it's described as "dummy" and non-functional in this context, RabbitMQ typically serves as a message broker or queuing agent to facilitate communication between different components of a distributed system.

5. **MySQL Database**:
   - MySQL is used as the database management system to store user information, including login details. The web application interacts with the MySQL database to perform user authentication and data retrieval operations.

6. **Memcached**:
   - Memcached is employed as a caching mechanism to improve the performance of the application. It caches frequently accessed data from the MySQL database, such as user login details, to reduce the need for repeated database queries.

7. **Flow of Execution**:
   - Users access the application through the browser by entering the URL.
   - Nginx manages incoming requests and distributes them to multiple instances of Tomcat.
   - Tomcat hosts the Java-based web application, interacting with MySQL for user data and Memcached for caching.
   - RabbitMQ, while non-functional in this scenario, would typically facilitate messaging between different components of the system.

Overall, the architectural design illustrates how the various components interact to provide a functional web application experience for users. It emphasizes the role of each component in handling different aspects of the application's functionality, from load balancing and request processing to data storage and caching.

<h2>Implementation Flow:</h2>

   - Setting up tools.
   - Cloning the source code repository.
   - Creating virtual machines.
   - Validating VMs and ensuring interactivity.
   - Setting up services sequentially: MySQL, Memcached, RabbitMQ, Tomcat, Nginx.
   - Building and deploying the Java application.
