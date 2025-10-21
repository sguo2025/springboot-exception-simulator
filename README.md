# Spring Boot Exception Simulator

一个用于模拟各种异常的 Spring Boot Demo：HTTP错误、延迟、OOM、CPU占用等。

## 运行

```bash
mvn spring-boot:run
```

或打包运行：

```bash
mvn package -DskipTests
java -jar target/springboot-exception-simulator-1.0.0.jar
```

## 接口示例

| URL | 说明 |
|------|-----|
| /simulate/runtime | 运行时异常 |
| /simulate/null | 空指针异常 |
| /simulate/delay | 延迟响应 |
| /simulate/oom | 模拟OOM |
| /simulate/cpu | 模拟CPU高占用 |
| /simulate/random | 随机异常 |
| /simulate/status/503 | 自定义HTTP状态码 |
| /actuator/prometheus | Prometheus指标 |
