# invesdwin-bom

This project consists of a BOM-POM ([bill of materials](https://maven.apache.org/guides/introduction/introduction-to-dependency-mechanism.html)) that can be used to share dependency management between multiple projects. It contains the versions for often used dependencies in invesdwin.

## Maven

Releases and snapshots are deployed to this maven repository:
```
http://invesdwin.de:8081/artifactory/invesdwin-oss
```

Dependency declaration:
```xml
<dependencyManagement>
	<dependencies>
		<dependency>
			<groupId>de.invesdwin</groupId>
			<artifactId>invesdwin-bom</artifactId>
			<version>1.0.0-SNAPSHOT</version>
			<type>pom</type>
			<scope>import</scope>
		</dependency>
	</dependencies>
</dependencyManagement>
```
