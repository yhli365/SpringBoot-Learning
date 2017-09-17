
Spring Boot基础教程
=============================
- https://github.com/dyc87112/SpringBoot-Learning
- http://blog.didispace.com/Spring-Boot基础教程/


CodeFix
=============================
# Chapter3-2-1
~~~
mysql>
use test;
create table USER(NAME VARCHAR(100) NOT NULL, AGE INT);
drop table USER;
~~~

# Chapter3-2-2
~~~
$ vi application.properties
spring.jpa.properties.hibernate.hbm2ddl.auto=create
~~~

# Chapter3-2-3
~~~
mysql>
create database test1;
create database test2;
create table test1.USER(ID bigint NOT NULL, NAME VARCHAR(100) NOT NULL, AGE INT, PRIMARY KEY (ID));
create table test2.USER(ID bigint NOT NULL, NAME VARCHAR(100) NOT NULL, AGE INT, PRIMARY KEY (ID));
drop database test1;
drop database test2;
~~~

# Chapter3-2-4
~~~
mysql>
create database test1;
create database test2;
drop database test1;
drop database test2;
~~~

# Chapter3-2-5
~~~
@test redis-3.2
cmd>
redis-server redis.windows.conf
redis-cli keys *
~~~

# Chapter3-2-6
~~~
@test mongodb-3.4.9
cmd>
# 设置用户密码
mongod --dbpath d:\ydata\mongodb\db
mongo 127.0.0.1:27017/test
> db.dropUser("name")
> db.createUser({user:"name",pwd:"pass",roles:[ { role: "readWrite", db: "test" }]})
# 以用户验证模式启动
mongod --dbpath d:\ydata\mongodb\db --auth
mongo 127.0.0.1:27017/test
> db.auth("name","pass")
0：代表授权失败 1：代表授权成功
> show collections
> exit
~~~

# Chapter3-2-7
# Chapter3-2-8
~~~
mysql>
create table test.USER(ID bigint auto_increment, NAME VARCHAR(100) NOT NULL, AGE INT NOT NULL, PRIMARY KEY (ID));
drop table test.USER;
~~~

