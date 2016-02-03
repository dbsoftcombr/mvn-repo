DBSoft Maven Repository

Configuração do **pom.xml** no seu projeto.

```
<properties>
	<dbssdk.version>2.0.2</dbssdk.version>
	<dbsfaces.version>2.0.2</dbsfaces.version>
	<jsf.version>2.2.11</jsf.version>
</properties>

<repositories>
	<repository>
		<id>dbsoftcombr-mvn-repo</id>
		<name>DBSoft.com.br Repository for Maven</name>
		<url>https://raw.github.com/dbsoftcombr/mvn-repo/master</url>
		<layout>default</layout> 
		<releases>
			<updatePolicy>daily</updatePolicy>
		</releases>
		<snapshots>
			<enabled>true</enabled>
			<updatePolicy>always</updatePolicy>
		</snapshots>			
	</repository>
	<repository>
		<id>central</id>
		<name>Maven Central Repository</name>
		<url>http://repo1.maven.org/maven2</url>
		<layout>default</layout>
	</repository>
<repositories>
```

```
<dependencies>
	<dependency>
		<groupId>br.com.dbsoft</groupId>
		<artifactId>dbsfaces</artifactId>
		<version>${dbsfaces.version}</version>
	</dependency>
</dependencies>
```
Não é necessário incluir a *dependency* do **dbssdk** quando utilizar o **dbsfaces**.

```
<dependencies>
	<dependency>
		<groupId>br.com.dbsoft</groupId>
		<artifactId>dbssdk</artifactId>
		<version>${dbssdk.version}</version>
	</dependency>
</dependencies>
```