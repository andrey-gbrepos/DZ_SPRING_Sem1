# DZ_SPRING_Sem1
## Создание проекта  - Основные команды:

- выбор архитипа, формирование проекта
	### mvn archetype: generate 
![Формирование проекта](images/settings_maven_project.png)

- компиляция проекта
	### mvn package 
![Компиляция проекта](images/compile_project.png)

- запуск файла .jar
	### java -jar myjar.jar - запуск файла .jar
![Запуск файла .jar](images/run_project.png)

## Плагины (pom.xml)
* Манифест
```
<plugin>
	<groupId>org.apache.maven.plugins</groupId>
	<artifactId>maven-jar-plugin</artifactId>
	<version>2.4</version>
	<configuration>
	  <archive>
	    <manifest>
		<mainClass>ru.gb.App</mainClass>
	    </manifest>
	  </archive>
	</configuration>
</plugin>
```
* Имя файла .jar

```
<plugin>
    <groupId>org.apache.maven.plugins</groupId>
   	<artifactId>maven-jar-plugin</artifactId>
   	<version>2.3.2</version>
    	<configuration>
      		<finalName>myjar</finalName>                   
   		</configuration>
</plugin>  
```

