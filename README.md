# WIN Backend Engineering Interview

## General Info

language used: NodeJs
framework used: Express
database: MongoDb 

## Setup
- clone the repo
- create .env file and paste all constants from dotenv-example file
- start mongodb server.
- run "npm i" to install packages
- run "npm start" to start server
- run "npm test" to run test cases


## How it works

REST Endpoints 
server: localhost:3000

## Service

1. To Add the new service : http://localhost:3000/service/create

2. To List All the service: http://localhost:3000/service/all
    
3. To Update the service : http://localhost:3000/service/update/:id

  
4. To Delete the service with : http://localhost:3000/service/delete/:id
    
5. To Get the service with id : http://localhost:3000/service/:id

## Orders

1. To Add the Order : http://localhost:3000/order/create

2. To List All the Orders: http://localhost:3000/order/all
    
3. To Update the Order : http://localhost:3000/order/update/:id

  
4. To Delete the Order with : http://localhost:3000/order/delete/:id
    
5. To Get the Order with id : http://localhost:3000/order/:id
## Scripts
start: npm start
test: npm test

## Structure

service: {
	serviceId: int,
	serviceName: string
}

order: {
	orderId: int,
        orderTime: timestamp,
        billAmount: int,
        services: [
        	{
                    id: int (linked to service)
                }
        ]
}

## Changes for production
- Add security
- Better logging implementation
- More test cases
- Db indexing
- use .env file for server and DB constants





5