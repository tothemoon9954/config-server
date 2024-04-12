# config-server



## config server 관리

1. ServerApplication에 @EnableConfigServer 추가
2. 파일 경로, branch, github에서 ssh 주소 가져오기
3. 대칭키, 비대칭키로 암호화가 가능, 지금은 대칭키로 해놓음



## server pom에 추가해놔야 할것들

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

### 암호화
![암호화](/image/암호화.png)

### 복호화
![복호화](/image/복호화.png)


### file repo를 private로 변환할 경우
1. git 계정의 settings -> SSH and GPG Keys -> New SSH Key
2. 이름은 마음대로 정하고 value는 터미널에서 
 cat 키파일명.pub을 해서 ssa부터 끝까지 전부다 등록
