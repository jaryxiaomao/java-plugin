# java-plugin
java一些有用的插件使用介绍

## mybatis-generator的使用
将相关第三方jar包信息和插件信息加入到pom文件中  

```
<dependency>
    <groupId>org.mybatis.generator</groupId>
    <artifactId>mybatis-generator-core</artifactId>
    <version>1.3.2</version>
</dependency>

<plugin>
    <groupId>org.mybatis.generator</groupId>
    <artifactId>mybatis-generator-maven-plugin</artifactId>
    <version>1.3.2</version>
    <configuration>
　　　　　　　<!-- mybatis用于生成代码的配置文件 -->
    　　<configurationFile>src/main/resources/generatorConfig.xml</configurationFile>
        <verbose>true</verbose>
        <overwrite>true</overwrite>
    </configuration>
</plugin>
```

eclipse中右击项目 maven build 中添加命令 mybatis-generator:generate  
idea右边maven项目打包命令中选择mybatis-generator如下图  
![gg](https://github.com/jaryxiaomao/java-plugin/blob/master/images/mybatis-generator.png)

