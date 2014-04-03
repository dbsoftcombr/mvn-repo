DBSoft Maven Repository

Configuração do **pom.xml** no seu projeto.

```
<repositories>
	<repository>
		<id>dbsoftcombr-mvn-repo</id>
		<name>DBSoft.com.br Repository for Maven</name>
		<url>https://raw.github.com/dbsoftcombr/mvn-repo/master</url>
		<layout>default</layout> 
		<releases>
			<updatePolicy>always</updatePolicy>
		</releases>
		<snapshots>
			<enabled>true</enabled>
			<updatePolicy>always</updatePolicy>
		</snapshots>			
	</repository>
<repositories>
```

```
<dependencies>
  <dependency>
  	<groupId>br.com.dbsoft</groupId>
  	<artifactId>dbsfaces</artifactId>
  	<version>1.0.0</version>
  </dependency>
</dependencies>
```
Não é necessário incluir a *dependency* do **dbssdk** quando utilizar o **dbsfaces**.

```
<dependencies>
  <dependency>
  	<groupId>br.com.dbsoft</groupId>
  	<artifactId>dbssdk</artifactId>
  	<version>1.0.0</version>
  </dependency>
</dependencies>
```

