DBSoft Maven Repository

Configuração do **pom.xml** no seu projeto.

```
<repository>
	<id>dbsoftcombr-mvn-repo</id>
	<name>DBSoft.com.br Repository for Maven</name>
	<url>https://github.com/dbsoftcombr/mvn-repo/raw/master/</url>
	<layout>default</layout> 
	<releases>
		<updatePolicy>always</updatePolicy>
	</releases>
	<snapshots>
		<enabled>true</enabled>
		<updatePolicy>always</updatePolicy>
	</snapshots>			
</repository>
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

