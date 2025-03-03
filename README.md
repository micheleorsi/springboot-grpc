# Spring Boot gRPC

[start.spring.io](https://start.spring.io) selection:

<img width="1685" alt="Screenshot 2025-03-03 at 10 46 50" src="https://github.com/user-attachments/assets/1f3479dc-cda1-461f-b0d1-a2f657b3ce1d" />


```
 ./gradlew bootRun
```

```

> Task :bootRun FAILED

  .   ____          _            __ _ _
 /\\ / ___'_ __ _ _(_)_ __  __ _ \ \ \ \
( ( )\___ | '_ | '_| | '_ \/ _` | \ \ \ \
 \\/  ___)| |_)| | | | | || (_| |  ) ) ) )
  '  |____| .__|_| |_|_| |_\__, | / / / /
 =========|_|==============|___/=/_/_/_/

 :: Spring Boot ::                (v3.4.3)

2025-03-03T11:08:05.204Z  INFO 6421 --- [demo] [           main] com.example.demo.DemoApplicationKt       : Starting DemoApplicationKt using Java 21.0.6 with PID 6421 (/Users/<user>/Development/springboot-grpc/build/classes/kotlin/main started by <user> in /Users/<user>/Development/springboot-grpc)
2025-03-03T11:08:05.205Z  INFO 6421 --- [demo] [           main] com.example.demo.DemoApplicationKt       : No active profile set, falling back to 1 default profile: "default"
2025-03-03T11:08:05.589Z  WARN 6421 --- [demo] [           main] s.c.a.AnnotationConfigApplicationContext : Exception encountered during context initialization - cancelling refresh attempt: org.springframework.beans.factory.BeanCreationException: Error creating bean with name 'org.springframework.boot.actuate.autoconfigure.metrics.task.TaskExecutorMetricsAutoConfiguration': Injection of autowired dependencies failed
2025-03-03T11:08:05.597Z  INFO 6421 --- [demo] [           main] .s.b.a.l.ConditionEvaluationReportLogger : 

Error starting ApplicationContext. To display the condition evaluation report re-run your application with 'debug' enabled.
2025-03-03T11:08:05.605Z ERROR 6421 --- [demo] [           main] o.s.b.d.LoggingFailureAnalysisReporter   : 

***************************
APPLICATION FAILED TO START
***************************

Description:

An attempt was made to call a method that does not exist. The attempt was made from the following location:

    org.springframework.boot.actuate.autoconfigure.metrics.task.TaskExecutorMetricsAutoConfiguration.bindTaskExecutorsToRegistry(TaskExecutorMetricsAutoConfiguration.java:60)

The following method did not exist:

    'java.util.Map org.springframework.beans.factory.support.SimpleAutowireCandidateResolver.resolveAutowireCandidates(org.springframework.beans.factory.config.ConfigurableListableBeanFactory, java.lang.Class)'

The calling method's class, org.springframework.boot.actuate.autoconfigure.metrics.task.TaskExecutorMetricsAutoConfiguration, was loaded from the following location:

    jar:file:/Users/<user>/.gradle/caches/modules-2/files-2.1/org.springframework.boot/spring-boot-actuator-autoconfigure/3.4.3/7687349974634acfe2bd65d31dd77ce739a29e62/spring-boot-actuator-autoconfigure-3.4.3.jar!/org/springframework/boot/actuate/autoconfigure/metrics/task/TaskExecutorMetricsAutoConfiguration.class

The called method's class, org.springframework.beans.factory.support.SimpleAutowireCandidateResolver, is available from the following locations:

    jar:file:/Users/<user>/.gradle/caches/modules-2/files-2.1/org.springframework/spring-beans/6.2.1/ab57ec03ba6900075bf28e3cd70ccce173205b8d/spring-beans-6.2.1.jar!/org/springframework/beans/factory/support/SimpleAutowireCandidateResolver.class

The called method's class hierarchy was loaded from the following locations:

    org.springframework.beans.factory.support.SimpleAutowireCandidateResolver: file:/Users/<user>/.gradle/caches/modules-2/files-2.1/org.springframework/spring-beans/6.2.1/ab57ec03ba6900075bf28e3cd70ccce173205b8d/spring-beans-6.2.1.jar


Action:

Correct the classpath of your application so that it contains compatible versions of the classes org.springframework.boot.actuate.autoconfigure.metrics.task.TaskExecutorMetricsAutoConfiguration and org.springframework.beans.factory.support.SimpleAutowireCandidateResolver


[Incubating] Problems report is available at: file:///Users/<user>/Development/springboot-grpc/build/reports/problems/problems-report.html

FAILURE: Build failed with an exception.

* What went wrong:
Execution failed for task ':bootRun'.
> Process 'command '/Library/Java/JavaVirtualMachines/<jvm>/Contents/Home/bin/java'' finished with non-zero exit value 1

* Try:
> Run with --stacktrace option to get the stack trace.
> Run with --info or --debug option to get more log output.
> Run with --scan to get full insights.
> Get more help at https://help.gradle.org.

Deprecated Gradle features were used in this build, making it incompatible with Gradle 9.0.

You can use '--warning-mode all' to show the individual deprecation warnings and determine if they come from your own scripts or plugins.

For more on this, please refer to https://docs.gradle.org/8.12.1/userguide/command_line_interface.html#sec:command_line_warnings in the Gradle documentation.

BUILD FAILED in 1s
7 actionable tasks: 2 executed, 5 up-to-date

```
