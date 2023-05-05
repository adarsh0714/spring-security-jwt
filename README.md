# spring-security-jwt
Spring Security JWT Authentication and Authorisation Project

## Tech Stack
- Java 17
- Spring Boot 3.0.6
- Maven
- PostgreSQL
- Flyway

### Implementation Summary

###### 01. setup spring security jwt
- setup database
- User(implements UserDetails from Spring Security), User Repository and Role
- JwtService -> To generate token, check token validity, extract claims
- JwtAuthenticationFilter -> To extract token, then username, and set context
- Application Config -> keep configs, starts at run time
- Security Config -> Enables Security, exclude few endpoints
- AuthController & AuthService -> for endpoints `/register` and `/authenticate`


### Run locally
- On the host, from IDE:
```
select appropriate branch and run:
  1 -> docker-compose.yml
  2 -> JavaSpringBootProjectsApplication.main
```