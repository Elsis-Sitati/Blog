---
layout: post
title: The four most important REST API methods
---

Rest API's Use HTTP methods to map CRUD (create, retrieve, update, delete) operations to HTTP requests.
The four most important used with API'S are GET,POST,PUT and DELETE

GET
Get is used to retrieve information e.g retrieve an address from a database.GET requests must be safe and idempotent,
meaning regardless how many times it repeats with the same parameters, the results are the same.

POST
Requests that the resources at the URL  do something with the provided entity.Often POST is use to create a new entity but
it can also be used to update an entity.However,it is not recommended to use POST to update already created data fields.
POST is best used to create new data entities.E.g creating a new student profile

PUT
Is used to store an entity.PUT can also be used to create or update an entity.The main difference between PUT and POST
is that PUT is idempotent while POST is not.Idempotent means that no matter how many times requests are made with same
parameters results must be the  same.PUT is best used to update already created data fields.

DELETE
Requests that a source may be removed. E.g removing a student's profile from a database



