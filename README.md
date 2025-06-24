# 🔗 TinyURL - Big Data URL Shortener

TinyURL is a Backend Java + Spring Boot application that shortens long URLs, tracks user clicks, and stores the data using scalable **Big Data** technologies like:

- 🟢 **MongoDB** — stores user click data  
- 🟣 **Cassandra** — stores user accounts and shortened URLs  
- 🔴 **Redis** — can be used for fast access/caching layer  

---

## 🌐 Live Demo

You can test the project **live** using Swagger UI here:  
👉 [https://binny-tinyurlbinny.runmydocker-app.com/swagger-ui.html](https://binny-tinyurlbinny.runmydocker-app.com/swagger-ui.html)

> You can create users, shorten URLs, and track clicks — all from the browser.

---

## 🧰 Tech Stack

| Layer        | Technology          |
|--------------|---------------------|
| Backend      | Spring Boot (Java)  |
| Database     | MongoDB, Cassandra  |
| Cache/Memory | Redis               |
| API Docs     | Swagger UI          |
| Container    | Docker + Docker Compose |

### :hammer_and_wrench: Languages and Tools :
<div>
  <img src="https://github.com/devicons/devicon/blob/master/icons/mongodb/mongodb-original-wordmark.svg" title="mongoDB" **alt="MongoDB" width="60" height="60"/>
  <img src="https://github.com/devicons/devicon/blob/master/icons/redis/redis-original-wordmark.svg" title="redis" **alt="redis" width="60" height="60"/>
  <img src="https://github.com/devicons/devicon/blob/master/icons/cassandra/cassandra-original-wordmark.svg" title="cassandra" **alt="cassandra" width="60" height="60"/>
  <img src="https://github.com/devicons/devicon/blob/master/icons/swagger/swagger-original-wordmark.svg" title="swagger"  alt="swagger" width="60" height="60"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/docker/docker-plain.svg" title="Docker" **alt="Docker" width="60" height="60"/> 
  <img src="https://github.com/devicons/devicon/blob/master/icons/spring/spring-original-wordmark.svg" title="spring" **alt="spring" width="60" height="60"/>
  <img src="https://github.com/devicons/devicon/blob/master/icons/java/java-original-wordmark.svg" title="Java" **alt="Java" width="60" height="60"/>
  <img src="https://github.com/devicons/devicon/blob/master/icons/intellij/intellij-original.svg" title="intellij" **alt="intellij" width="60" height="60"/>
</div>

---

## ⚙️ Run Locally

### 1. 🔽 Clone the project

```bash
git clone https://github.com/YOUR_USERNAME/tinyurl.git
cd tinyurl
```

### 2. 🐳 Start Databases with Docker Compose
```bash
Run the following command to spin up MongoDB, Cassandra, and Redis using Docker:

bash
Copy
Edit
docker-compose up -d
This starts:

🟢 MongoDB on port 27017

🟣 Cassandra on port 9042

🔴 Redis on port 6379
```
### 3. 🏗️ Build the Project with Maven
```bash
If you’re using the Maven Wrapper:

bash
Copy
Edit
./mvnw clean package
Or with Maven installed:

bash
Copy
Edit
mvn clean package
This will generate a .jar file inside the target/ folder.
```
### 4. 📦 Build the Docker Image
```bash
Use the Dockerfile in the root of the project to build the image:

bash
Copy
Edit
docker build -t tinyurl .
```
### 5. 🚀 Run the Application Container
```bash
Launch the application using:

bash
Copy
Edit
docker run -p 8080:8080 tinyurl
This exposes the app on http://localhost:8080

To access the Swagger UI:

bash
Copy
Edit
http://localhost:8080/swagger-ui.html
Or visit the deployed version:

👉 https://binny-tinyurlbinny.runmydocker-app.com/swagger-ui.html
```


