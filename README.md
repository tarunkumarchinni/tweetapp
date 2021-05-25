# tweetapp
java based application

if using mysql

create table user(id int(50) not null auto_increment primary key,FIRST_NAME varchar(255), LAST_NAME varchar(255), GENDER varchar(255), DOB varchar(255), EMAIL varchar(255), PASSWORD varchar(255))


create table tweets(USER_ID varchar(255), TWEET varchar(255), INSERT_DTS varchar(255));

app.properties

spring.jpa.database-platform=org.hibernate.dialect.H2Dialect
spring.h2.console.enabled=true
spring.h2.console.path=/h2
spring.jpa.hibernate.ddl-auto=none
spring.datasource.url=jdbc:mysql://localhost:3306/tweetappdb
spring.datasource.username=root
spring.datasource.password=root


pom.xml
remove h2 dependency
add mysql below
<dependency>
		    <groupId>mysql</groupId>
		    <artifactId>mysql-connector-java</artifactId>
		</dependency>
