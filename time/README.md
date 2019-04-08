# time

本module使用spring boot来实现rest接口。

参考教程[Building a RESTful Web Service](https://spring.io/guides/gs/rest-service/).

由于已经有了parent pom，故不再使用教程中的方式直接继承`spring-boot-starter-parent`，而是参考[Using Spring Boot without the Parent POM](https://docs.spring.io/spring-boot/docs/current/reference/html/using-boot-build-systems.html#using-boot-maven-without-a-parent)的方式导入了相关依赖：

```xml
<dependencyManagement>
	<dependencies>
		<dependency>
			<!-- Import dependency management from Spring Boot -->
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-dependencies</artifactId>
			<version>2.1.4.RELEASE</version>
			<type>pom</type>
			<scope>import</scope>
		</dependency>
	</dependencies>
</dependencyManagement>
```

参考[Spring Boot with No Parent – Example](https://www.surasint.com/spring-boot-with-no-parent-example/)解决编译相关的其他问题。
