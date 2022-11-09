# Spring Boot Security Login Demo with JWT and H2

- Appropriate Flow for User Login and Registration with JWT and HttpOnly Cookie
- Spring Boot Rest Api Architecture with Spring Security

```
## Run Spring Boot application
```
mvn spring-boot:run
```

## Post Man CURL command for singin and singup

# SingUp
```
curl --location --request POST 'localhost:8080/api/auth/signup' \
--header 'Content-Type: application/json' \
--header 'Cookie: bezkoder=eyJhbGciOiJIUzUxMiJ9.eyJzdWIiOiJhcnVuIiwiaWF0IjoxNjY3ODk0NDAxLCJleHAiOjE2Njc5ODA4MDF9.ddSbSJSgkSQvpeWETRxr1BaoQSZPvKtfwe3t3P53P55YTRLm8778OKUQBGc9p7HsvtLlE6zpcelih-17WULy_g; spring-demo-app-cookie=eyJhbGciOiJIUzUxMiJ9.eyJzdWIiOiJhcnVuIiwiaWF0IjoxNjY3ODk2NjY5LCJleHAiOjE2Njc5ODMwNjl9.Wy99rRJgE-EABfJLqJjUoiyVrp033gASNBqd2TtgwIJUzEb4vL425F-DTjwbumKINWmYtrpt7L8e-pmc5AAjpg' \
--data-raw '{
    "username": "arun",
    "email": "arun@gmail.com",
    "password": "arun123"
}'
```
 
# SignIn 
```
curl --location --request POST 'localhost:8080/api/auth/signin' \
--header 'Content-Type: application/json' \
--header 'Cookie: bezkoder=eyJhbGciOiJIUzUxMiJ9.eyJzdWIiOiJhcnVuIiwiaWF0IjoxNjY3ODk0NDAxLCJleHAiOjE2Njc5ODA4MDF9.ddSbSJSgkSQvpeWETRxr1BaoQSZPvKtfwe3t3P53P55YTRLm8778OKUQBGc9p7HsvtLlE6zpcelih-17WULy_g; spring-demo-app-cookie=eyJhbGciOiJIUzUxMiJ9.eyJzdWIiOiJhcnVuIiwiaWF0IjoxNjY3ODk2NjY5LCJleHAiOjE2Njc5ODMwNjl9.Wy99rRJgE-EABfJLqJjUoiyVrp033gASNBqd2TtgwIJUzEb4vL425F-DTjwbumKINWmYtrpt7L8e-pmc5AAjpg' \
--data-raw '{
    "username": "arun",
    "password": "arun"
}'
```