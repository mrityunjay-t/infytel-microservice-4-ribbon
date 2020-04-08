# infytel-microservice-4-ribbon

This repository contains Infytel Application depicting basic micro service architecture containing.

All applications have different database.

The cloud configurations are fetched using bootstrap.properties from Git Repository.

Configurations can be updated in runtime:

Add actuator-refresh dependency in pom.xml file for the MS in which we want to update configs in runtime
Send a post request to http://URL/actuator/refresh
Example for CustomerMS in this project:
A POST request to: http://localhost:8200/actuator/refresh

Ribbon Application: We will be using ribbon for FriendFamilyMS on port 8300 and 8301 for load balancing with Eureka.

We have four microservices CallDetailsMS, CustomerMS, FriendsFamilyMS and PlanMS.

CallDetailsMS: Contains call details for Customers.

PlanMS: Contains details for Customer Plan

FriendFamilyMS: Details of friends and family for Customers

CustomerMS: All details for customer including, Call Details, Plan, FriendFamily.
