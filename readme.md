Есть три части:
1. Eureka Server - port: 8761
2. Client Service - port: 8081
3. Gateway Service - 4444

При запросе на http://localhost:4444/api/client/something перебрасывает на http://localhost:8081/api/client/something. 
Но перебрасывает он только в том случае, если при запросе на http://localhost:4444/api/client/something ты указываешь заголовок spring-cloud-course.
