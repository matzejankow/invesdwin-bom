# invesdwin-bom

This project consists of a BOM-POM ([bill of materials](https://maven.apache.org/guides/introduction/introduction-to-dependency-mechanism.html)) that can be used to share dependency management between multiple projects. It contains the versions for often used dependencies in invesdwin.

## Maven

Releases and snapshots are deployed to this maven repository:
```
https://invesdwin.de/repo/invesdwin-oss-remote
```

Dependency declaration:
```xml
<dependencyManagement>
	<dependencies>
		<dependency>
			<groupId>de.invesdwin</groupId>
			<artifactId>invesdwin-bom</artifactId>
			<version>1.0.13</version><!---project.version.invesdwin-bom-->
			<type>pom</type>
			<scope>import</scope>
		</dependency>
	</dependencies>
</dependencyManagement>
```

## Support

If you need further assistance or have some ideas for improvements and don't want to create an issue here on github, feel free to start a discussion in our [invesdwin-platform](https://groups.google.com/forum/#!forum/invesdwin-platform) mailing list.
