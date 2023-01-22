
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

