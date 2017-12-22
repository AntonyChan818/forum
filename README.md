###### df
###### 一个简单的论坛系统
1. 该项目开发IDE为IntelliJ IDEA，通过Maven构建，后台采用Spring、SpringMVC、MyBatis，数据库采用MySQL、Redis，前台用到jQuery，图片被上传到七牛云。
2. 在mysql创建数据df，字符集utf-8，运行df.sql。
3. 修改df.properties中的mysql.password，redis.password，mail.password为您个人的配置。
 
```
  mysql.url=jdbc:mysql://127.0.0.1:3306/df
  mysql.driverClassName=com.mysql.jdbc.Driver
  mysql.username=root
  mysql.password=root

  redis.hostName=127.0.0.1
  redis.port=6379
  redis.timeout=5000
```
如上，若redis无密码，则可将redis.password去除，并将\src\main\resources\application-context.xml中，42行去除。


```
  <!--Redis密码-->
  <!--<constructor-arg index="4" value="${redis.password}" />-->
```

4. 此项目为初学者练手项目，仅为交流，有什么错误希望大家能指出，在此感谢。
