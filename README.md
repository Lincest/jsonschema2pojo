# jsonschema2pojo: add [fastjson](https://github.com/alibaba/fastjson) support in maven-plugin

## installation

```shell
mvn clean install 
```

## usage

```xml
<plugin>
    <groupId>org.jsonschema2pojo</groupId>
    <artifactId>jsonschema2pojo-maven-plugin</artifactId>
    <version>1.1.5-SNAPSHOT</version>
    <configuration>
        <sourceDirectory>${basedir}/src/main/resources/schema</sourceDirectory>
        <targetPackage>com.example.types</targetPackage>
        <annotationStyle>fastjson</annotationStyle>
    </configuration>
    <executions>
        <execution>
            <goals>
                <goal>generate</goal>
            </goals>
        </execution>
    </executions>
</plugin>
```