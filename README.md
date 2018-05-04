# AuthServerDemo
A demo Spring Boot application to demonstrate OAuth2 of Spring Security in Java.

# About
AuthServerDemo is an small application to demonstrate how to use an Oauth2 Services to build a simple Auth Server.

# Prerequisites
1.Java 2.Spring Boot 3.Spring Security 4. Gradle 5. Postman

# Request 
curl -X POST \
  http://localhost:8080/oauth/token \
  -H 'Authorization: Basic Y2xpZW50OmNsaWVudFNlY3JldA==' \
  -H 'Cache-Control: no-cache' \
  -H 'Content-Type: application/x-www-form-urlencoded' \
  -H 'Postman-Token: e52d1a4f-69e6-1fb7-3d43-b83de93c9e14' \
  -d 'client_id=client&username=user&password=user&grant_type=password'

# What is Authentication Server ?
An authentication server is an application that facilitates authentication of an entity that attempts to access a network. Such an entity may be a human user or another server. It genrates a token which is passed for Authentication of User.

# How can we build an Auth Server using Spring Security ?
In this application we are using some basic jars(web,security, oauth2)provided by Spring Framework. Spring security provides way to secure application based on Spring Filter Chain Processing.

# What is Spring Filter Chain ?
Spring Security maintains a filter chain internally where each of the filters has a particular responsibility and filters are added or removed from the configuration depending on which services are required.

