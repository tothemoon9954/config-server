# config-server



config server 관리

1. ServerApplication에 @EnableConfigServer 추가
2. 파일 경로, branch, github에서 ssh 주소 가져오기
3. 대칭키, 비대칭키로 암호화가 가능, 지금은 대칭키로 해놓음

server pom에 추가해놔야 할것들

		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-actuator</artifactId>
		</dependency>
  
		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-web</artifactId>
		</dependency>
  
		<dependency>
			<groupId>org.springframework.cloud</groupId>
			<artifactId>spring-cloud-config-server</artifactId>
		</dependency>
