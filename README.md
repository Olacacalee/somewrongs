# somewrongs


> 1. com.spotify:docker-maven-plugin 报localhost:2375 Connection refused 错误
```
使用maven的docker插件时候，编译时会报如下错误：

Failed to execute goal com.spotify:docker-maven-plugin:0.2.9:build (default-cli) on project config: Exception caught: java.util.concurrent.ExecutionException: com.spotify.docker.client.shaded.javax.ws.rs.ProcessingException: org.apache.http.conn.HttpHostConnectException: Connect to localhost:2375 [localhost/127.0.0.1, localhost/0:0:0:0:0:0:0:1] failed: Connection refused


解决办法：

把docker-maven-plugin版本更新成0.4.13即可
```
