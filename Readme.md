# REST API


## Audiance

The target audiance of this project is the the Teachr recruitment team

## High level overview

This deliverable consists of the creation of Resful API using API Platform.

## The HTTP requests supported are

#### GET

###### GET by ID: 
	
Returns an object using the object ID

Request body:
```
{
  'id':'id_value',
}
```
API PATH: 
>/api/clients/{id}
###### GET all:

Returns all objects contained in the database

Request body: Empty

API PATH: 
>/api/clients

#### POST

The post request creates a complete object using the name (string)

Request body:
```	
{
 'name': 'string',
}
```
API PATH: 
>/api/clients

#### DELETE

The delete request aims to delete an object using its ID

Request body:

```
{
  'id':'id_value',
}
```
API PATH: 
> /api/clients/{id}
#### Setup

1. Database creation
```
bin/console doctrine:database:create
```

2. Set the database table
```
bin/console doctrine:schema:create
```
  
