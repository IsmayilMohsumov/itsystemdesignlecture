
# IT Sytem design 

User Management System with Microservices architecure the project contains 7 (seven) microservices and each of them serves for different purposes. I will describe all of them seperately within details.


## Tech Stack

**Java Spring,** **Maven,** **Zipkin,** **Postgres,** **Docker,** 
**RabbitMQ**



## Run Locally

Clone the project

```bash
  git clone https://link-to-project
```

Go to the project directory

```bash
  cd my-project
```

Run images

```bash
  docker compose up -d
```

Start the server

```bash
  Send POST request to: 
  
  localhost:8083/api/v1/customers
  
  with body:

  {
    "firstName":"itsystemdesign",
    "lastName":"lecture",
    "email":"aeh@vizja.pl"
}
```

## Architecture

![img_1.png](img_1.png)

## Project in action

1. Run images

```bash
  docker compose up -d
```
![img_2.png](img_2.png)

2. Check logs for **customer**

```bash
  docker logs customer
```
![img_3.png](img_3.png)

3. Send request using postman

#### Get all items

```http
  POST /api/v1/customers
  
  {
    "firstName":"itsystemdesign",
    "lastName":"mohsum2ov",
    "email":"ismayi2l@gmail.com"
}
```

| Parameter | Type   | Description        |
|:----------|:-------|:-------------------|
| `raw`     | `JSON` | **Required**. Body |

![img_5.png](img_5.png)

4. Check logs using **zipkin**

#### Open browser and search for http://localhost:9411/zipkin/

![img_4.png](img_4.png)


5. Check database

#### Open browser and search for http://localhost:5050/browser/

![img_6.png](img_6.png)