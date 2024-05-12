# random
win thì thêm dòng au vào setenv.bat và setenv32.bat

``` 
set JAVA_OPTS=-javaagent:"C:\Program Files\Atlassian\Application Data\Jira\agent.jar" %JAVA_OPTS% '
set CATALINA_OPTS=-javaagent:"C:\Program Files\Atlassian\Application Data\Jira\agent.jar" %CATALINA_OPTS%
```
Theemn vào environment variables của win


| Hàm | Giá Trị |
|-----|---------|
|JAVA_OPTS |  -javaagent:"C:\Program Files\Atlassian\Application Data\Jira\agent.jar |
| CATALINA_OPTS | -javaagent:"C:\Program Files\Atlassian\Application Data\Jira\agent.jar |

Tìm mở file: catalina.bat

```set CATALINA_OPTS=```

Thay toàn bộ bằng bằng

```set CATALINA_OPTS=-javaagent:"C:\Program Files\Atlassian\Application Data\Jira\agent.jar```