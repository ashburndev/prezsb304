On March 15 I visited https://start.spring.io/ and created a Spring Boot 3.0.4 web application named prezsb304.  This generated and downloaded the prezsb304.zip file.

    Project: Gradle - Groovy
    Language: Java
    Spring Boot: 3.0.4
    Group: ashburncode
    Artifact: prezsb304
    Name: prezsb304
    Description: Demo project for Spring Boot
    Package name: ashburncode.prezsb304
    Packaging: Jar
    Java: 17
    Dependencies:
      Spring Web Web
        Build web, including RESTful, applications using Spring MVC. Uses Apache Tomcat as the default embedded container.
      Spring Data JPA SQL
        Persist data in SQL stores with Java Persistence API using Spring Data and Hibernate.
      MySQL Driver SQL
        MySQL JDBC driver.
      Rest Repositories Web
        Exposing Spring Data repositories over REST via Spring Data REST.
      Spring Boot Actuator Ops
        Supports built in (or custom) endpoints that let you monitor and manage your application - such as application health, metrics, sessions, etc.

Once downloaded, I unzipped the file into the /home/davidho/sbootprojs directory.  Then I started Eclipse 2022-12 and imported the project (the youtube video below was very helpful in documenting that process).

    https://kenkousen.substack.com/about
    https://kenkousen.substack.com/archive
    https://kenkousen.substack.com/p/tales-from-the-jar-side-its-my-birthday

    https://www.youtube.com/watch?v=HbDiE9Bgaco
    Import Gradle Projects into Eclipse

I am using the jee version of Eclipse 2022-12.

    drwxr-xr-x  8 davidho davidho 4096 Dec  1 15:13 eclipse-java-2022-12-R-linux-gtk-x86_64
    drwxr-xr-x  8 davidho davidho 4096 Dec  1 15:29 eclipse-jee-2022-12-R-linux-gtk-x86_64

Here is a directory listing of the prezsb304 directory, and some additional information about the project.

    davidho@dphxps17:~$ ls -latr ~/Downloads/ | tail
    -rw-rw-r--  1 davidho davidho   42003461 Mar  8 10:30 Amazon_Web_Services_in_Action_Third_Edi_v10.pdf
    -rw-rw-r--  1 davidho davidho   41239678 Mar  8 10:30 Amazon_Web_Services_in_Action_Third_Edi_v10.epub
    -rw-rw-r--  1 davidho davidho   22878443 Mar  8 10:30 Amazon_Web_Services_in_Action_Third_Edi_v10.mobi
    -rw-rw-r--  1 davidho davidho   18806644 Mar  8 10:30 Amazon_Web_Services_in_Action_Third_Edi_v10.code3-main.zip
    -rw-rw-r--  1 davidho davidho      65167 Mar 14 06:26 sbapp304g.zip
    -rw-rw-r--  1 davidho davidho      65069 Mar 14 06:29 sbapp304m.zip
    -rw-rw-r--  1 davidho davidho    1093284 Mar 15 07:56 prezinfogaf.zip
    drwxr-x--- 56 davidho davidho       4096 Mar 15 15:58 ..
    -rw-rw-r--  1 davidho davidho      65157 Mar 15 17:23 prezsb304.zip
    drwxr-xr-x  6 davidho davidho      20480 Mar 15 17:23 .
    davidho@dphxps17:~$ 
    davidho@dphxps17:~$ cd ~/sbootprojs/
    davidho@dphxps17:~/sbootprojs$ ls -latr | tail
    drwxr-xr-x  4 davidho davidho   4096 Mar  2 19:34 sbapp303g
    drwxr-xr-x  4 davidho davidho   4096 Mar  2 19:36 sbapp303m
    -rw-rw-r--  1 davidho davidho  65167 Mar 14 06:26 sbapp304g.zip
    -rw-rw-r--  1 davidho davidho  65069 Mar 14 06:29 sbapp304m.zip
    drwxr-xr-x  4 davidho davidho   4096 Mar 14 10:26 sbapp304g
    drwxr-xr-x  4 davidho davidho   4096 Mar 14 10:28 sbapp304m
    drwxr-x--- 56 davidho davidho   4096 Mar 15 15:58 ..
    -rw-rw-r--  1 davidho davidho  65157 Mar 15 17:23 prezsb304.zip
    drwxrwxr-x 20 davidho davidho   4096 Mar 15 17:27 .
    drwxr-xr-x  4 davidho davidho   4096 Mar 15  2023 prezsb304
    davidho@dphxps17:~/sbootprojs$ 
    davidho@dphxps17:~/sbootprojs$ cd prezsb304/
    davidho@dphxps17:~/sbootprojs/prezsb304$ 
    davidho@dphxps17:~/sbootprojs/prezsb304$ ls -latr
    total 44
    drwxrwxr-x 20 davidho davidho 4096 Mar 15 17:27 ..
    drwxr-xr-x  4 davidho davidho 4096 Mar 15  2023 src
    -rw-r--r--  1 davidho davidho   31 Mar 15  2023 settings.gradle
    -rw-r--r--  1 davidho davidho 1900 Mar 15  2023 HELP.md
    -rw-r--r--  1 davidho davidho 2838 Mar 15  2023 gradlew.bat
    -rwxr-xr-x  1 davidho davidho 8188 Mar 15  2023 gradlew
    drwxr-xr-x  3 davidho davidho 4096 Mar 15  2023 gradle
    -rw-r--r--  1 davidho davidho  444 Mar 15  2023 .gitignore
    -rw-r--r--  1 davidho davidho  697 Mar 15  2023 build.gradle
    drwxr-xr-x  4 davidho davidho 4096 Mar 15  2023 .
    davidho@dphxps17:~/sbootprojs/prezsb304$ 
    davidho@dphxps17:~/sbootprojs/prezsb304$ find . -print
    .
    ./.gitignore
    ./gradle
    ./gradle/wrapper
    ./gradle/wrapper/gradle-wrapper.properties
    ./gradle/wrapper/gradle-wrapper.jar
    ./settings.gradle
    ./HELP.md
    ./src
    ./src/test
    ./src/test/java
    ./src/test/java/ashburncode
    ./src/test/java/ashburncode/prezsb304
    ./src/test/java/ashburncode/prezsb304/Prezsb304ApplicationTests.java
    ./src/main
    ./src/main/resources
    ./src/main/resources/static
    ./src/main/resources/application.properties
    ./src/main/resources/templates
    ./src/main/java
    ./src/main/java/ashburncode
    ./src/main/java/ashburncode/prezsb304
    ./src/main/java/ashburncode/prezsb304/Prezsb304Application.java
    ./build.gradle
    ./gradlew.bat
    ./gradlew
    davidho@dphxps17:~/sbootprojs/prezsb304$ 
    davidho@dphxps17:~/sbootprojs/prezsb304$ find . -type f -exec ls -la {} \;
    -rw-r--r-- 1 davidho davidho 444 Mar 15  2023 ./.gitignore
    -rw-r--r-- 1 davidho davidho 202 Mar 15  2023 ./gradle/wrapper/gradle-wrapper.properties
    -rw-r--r-- 1 davidho davidho 60756 Mar 15  2023 ./gradle/wrapper/gradle-wrapper.jar
    -rw-r--r-- 1 davidho davidho 31 Mar 15  2023 ./settings.gradle
    -rw-r--r-- 1 davidho davidho 1900 Mar 15  2023 ./HELP.md
    -rw-r--r-- 1 davidho davidho 216 Mar 15  2023 ./src/test/java/ashburncode/prezsb304/Prezsb304ApplicationTests.java
    -rw-r--r-- 1 davidho davidho 1 Mar 15  2023 ./src/main/resources/application.properties
    -rw-r--r-- 1 davidho davidho 320 Mar 15  2023 ./src/main/java/ashburncode/prezsb304/Prezsb304Application.java
    -rw-r--r-- 1 davidho davidho 697 Mar 15  2023 ./build.gradle
    -rw-r--r-- 1 davidho davidho 2838 Mar 15  2023 ./gradlew.bat
    -rwxr-xr-x 1 davidho davidho 8188 Mar 15  2023 ./gradlew
    davidho@dphxps17:~/sbootprojs/prezsb304$ 
    davidho@dphxps17:~/sbootprojs/prezsb304$ jar tvf ./gradle/wrapper/gradle-wrapper.jar
        0 Fri Feb 01 00:00:00 EST 1980 META-INF/
        63 Fri Feb 01 00:00:00 EST 1980 META-INF/MANIFEST.MF
        0 Fri Feb 01 00:00:00 EST 1980 org/
        0 Fri Feb 01 00:00:00 EST 1980 org/gradle/
        0 Fri Feb 01 00:00:00 EST 1980 org/gradle/wrapper/
      5677 Fri Feb 01 00:00:00 EST 1980 org/gradle/wrapper/GradleWrapperMain.class
        51 Fri Feb 01 00:00:00 EST 1980 gradle-wrapper-classpath.properties
        0 Fri Feb 01 00:00:00 EST 1980 gradle-wrapper-parameter-names.properties
        0 Fri Feb 01 00:00:00 EST 1980 org/gradle/cli/
      1363 Fri Feb 01 00:00:00 EST 1980 org/gradle/cli/AbstractCommandLineConverter.class
      2796 Fri Feb 01 00:00:00 EST 1980 org/gradle/cli/AbstractPropertiesCommandLineConverter.class
      587 Fri Feb 01 00:00:00 EST 1980 org/gradle/cli/CommandLineArgumentException.class
      615 Fri Feb 01 00:00:00 EST 1980 org/gradle/cli/CommandLineConverter.class
      3687 Fri Feb 01 00:00:00 EST 1980 org/gradle/cli/CommandLineOption.class
      229 Fri Feb 01 00:00:00 EST 1980 org/gradle/cli/CommandLineParser$1.class
      2495 Fri Feb 01 00:00:00 EST 1980 org/gradle/cli/CommandLineParser$AfterFirstSubCommand.class
      1830 Fri Feb 01 00:00:00 EST 1980 org/gradle/cli/CommandLineParser$AfterOptions.class
      2933 Fri Feb 01 00:00:00 EST 1980 org/gradle/cli/CommandLineParser$BeforeFirstSubCommand.class
      1263 Fri Feb 01 00:00:00 EST 1980 org/gradle/cli/CommandLineParser$CaseInsensitiveStringComparator.class
      4390 Fri Feb 01 00:00:00 EST 1980 org/gradle/cli/CommandLineParser$KnownOptionParserState.class
      1780 Fri Feb 01 00:00:00 EST 1980 org/gradle/cli/CommandLineParser$MissingOptionArgState.class
      1732 Fri Feb 01 00:00:00 EST 1980 org/gradle/cli/CommandLineParser$OptionAwareParserState.class
      1706 Fri Feb 01 00:00:00 EST 1980 org/gradle/cli/CommandLineParser$OptionComparator.class
      931 Fri Feb 01 00:00:00 EST 1980 org/gradle/cli/CommandLineParser$OptionParserState.class
      1462 Fri Feb 01 00:00:00 EST 1980 org/gradle/cli/CommandLineParser$OptionString.class
      1400 Fri Feb 01 00:00:00 EST 1980 org/gradle/cli/CommandLineParser$OptionStringComparator.class
      1208 Fri Feb 01 00:00:00 EST 1980 org/gradle/cli/CommandLineParser$ParserState.class
      1899 Fri Feb 01 00:00:00 EST 1980 org/gradle/cli/CommandLineParser$UnknownOptionParserState.class
    10604 Fri Feb 01 00:00:00 EST 1980 org/gradle/cli/CommandLineParser.class
      4608 Fri Feb 01 00:00:00 EST 1980 org/gradle/cli/ParsedCommandLine.class
      1349 Fri Feb 01 00:00:00 EST 1980 org/gradle/cli/ParsedCommandLineOption.class
      779 Fri Feb 01 00:00:00 EST 1980 org/gradle/cli/ProjectPropertiesCommandLineConverter.class
      764 Fri Feb 01 00:00:00 EST 1980 org/gradle/cli/SystemPropertiesCommandLineConverter.class
        0 Fri Feb 01 00:00:00 EST 1980 org/gradle/util/
        0 Fri Feb 01 00:00:00 EST 1980 org/gradle/util/internal/
      1319 Fri Feb 01 00:00:00 EST 1980 org/gradle/util/internal/ZipSlip.class
      793 Fri Feb 01 00:00:00 EST 1980 org/gradle/wrapper/BootstrapMainStarter$1.class
      2596 Fri Feb 01 00:00:00 EST 1980 org/gradle/wrapper/BootstrapMainStarter.class
      210 Fri Feb 01 00:00:00 EST 1980 org/gradle/wrapper/Download$1.class
      2008 Fri Feb 01 00:00:00 EST 1980 org/gradle/wrapper/Download$DefaultDownloadProgressListener.class
      1918 Fri Feb 01 00:00:00 EST 1980 org/gradle/wrapper/Download$ProxyAuthenticator.class
      9896 Fri Feb 01 00:00:00 EST 1980 org/gradle/wrapper/Download.class
      202 Fri Feb 01 00:00:00 EST 1980 org/gradle/wrapper/DownloadProgressListener.class
      3204 Fri Feb 01 00:00:00 EST 1980 org/gradle/wrapper/ExclusiveFileAccessManager.class
      1158 Fri Feb 01 00:00:00 EST 1980 org/gradle/wrapper/GradleUserHomeLookup.class
      219 Fri Feb 01 00:00:00 EST 1980 org/gradle/wrapper/IDownload.class
      4742 Fri Feb 01 00:00:00 EST 1980 org/gradle/wrapper/Install$1.class
      1561 Fri Feb 01 00:00:00 EST 1980 org/gradle/wrapper/Install$InstallCheck.class
    11647 Fri Feb 01 00:00:00 EST 1980 org/gradle/wrapper/Install.class
      1332 Fri Feb 01 00:00:00 EST 1980 org/gradle/wrapper/Logger.class
      751 Fri Feb 01 00:00:00 EST 1980 org/gradle/wrapper/PathAssembler$LocalDistribution.class
      3627 Fri Feb 01 00:00:00 EST 1980 org/gradle/wrapper/PathAssembler.class
      2428 Fri Feb 01 00:00:00 EST 1980 org/gradle/wrapper/SystemPropertiesHandler.class
      1855 Fri Feb 01 00:00:00 EST 1980 org/gradle/wrapper/WrapperConfiguration.class
      5148 Fri Feb 01 00:00:00 EST 1980 org/gradle/wrapper/WrapperExecutor.class
    davidho@dphxps17:~/sbootprojs/prezsb304$ 
    davidho@dphxps17:~/sbootprojs/prezsb304$ ./gradlew --version

    ------------------------------------------------------------
    Gradle 7.6.1
    ------------------------------------------------------------

    Build time:   2023-02-24 13:54:42 UTC
    Revision:     3905fe8ac072bbd925c70ddbddddf4463341f4b4

    Kotlin:       1.7.10
    Groovy:       3.0.13
    Ant:          Apache Ant(TM) version 1.10.11 compiled on July 10 2021
    JVM:          17.0.6 (Azul Systems, Inc. 17.0.6+10-LTS)
    OS:           Linux 5.19.0-35-generic amd64

    davidho@dphxps17:~/sbootprojs/prezsb304$ 


    File | Import... Gradle | Existing Gradle Project
      Project Root Director
        /home/davidho/sbootprojs/prezsb304

    Working Directory: /home/davidho/sbootprojs/prezsb304
    Gradle user home: /home/davidho/.gradle
    Gradle Distribution: Gradle wrapper from target build
    Gradle Version: 7.6.1
    Java Home: /opt/eclipse-jee-2022-12-R-linux-gtk-x86_64/plugins/org.eclipse.justj.openjdk.hotspot.jre.full.linux.x86_64_17.0.5.v20221102-0933/jre
    JVM Arguments: None
    Program Arguments: None
    Build Scans Enabled: false
    Offline Mode Enabled: false
    Gradle Tasks: bootRun

    > Task :compileJava
    > Task :processResources
    > Task :classes
    > Task :resolveMainClassName

    > Task :bootRun FAILED

      .   ____          _            __ _ _
    /\\ / ___'_ __ _ _(_)_ __  __ _ \ \ \ \
    ( ( )\___ | '_ | '_| | '_ \/ _` | \ \ \ \
    \\/  ___)| |_)| | | | | || (_| |  ) ) ) )
      '  |____| .__|_| |_|_| |_\__, | / / / /
    =========|_|==============|___/=/_/_/_/
    :: Spring Boot ::                (v3.0.4)

    2023-03-15T17:49:05.030-04:00  INFO 25057 --- [           main] a.prezsb304.Prezsb304Application         : Starting Prezsb304Application using Java 17.0.5 with PID 25057 (/home/davidho/sbootprojs/prezsb304/build/classes/java/main started by davidho in /home/davidho/sbootprojs/prezsb304)
    2023-03-15T17:49:05.032-04:00  INFO 25057 --- [           main] a.prezsb304.Prezsb304Application         : No active profile set, falling back to 1 default profile: "default"
    2023-03-15T17:49:05.380-04:00  INFO 25057 --- [           main] .s.d.r.c.RepositoryConfigurationDelegate : Bootstrapping Spring Data JPA repositories in DEFAULT mode.
    2023-03-15T17:49:05.391-04:00  INFO 25057 --- [           main] .s.d.r.c.RepositoryConfigurationDelegate : Finished Spring Data repository scanning in 5 ms. Found 0 JPA repository interfaces.
    2023-03-15T17:49:05.623-04:00  INFO 25057 --- [           main] o.s.b.w.embedded.tomcat.TomcatWebServer  : Tomcat initialized with port(s): 8080 (http)
    2023-03-15T17:49:05.628-04:00  INFO 25057 --- [           main] o.apache.catalina.core.StandardService   : Starting service [Tomcat]
    2023-03-15T17:49:05.629-04:00  INFO 25057 --- [           main] o.apache.catalina.core.StandardEngine    : Starting Servlet engine: [Apache Tomcat/10.1.5]
    2023-03-15T17:49:05.670-04:00  INFO 25057 --- [           main] o.a.c.c.C.[Tomcat].[localhost].[/]       : Initializing Spring embedded WebApplicationContext
    2023-03-15T17:49:05.671-04:00  INFO 25057 --- [           main] w.s.c.ServletWebServerApplicationContext : Root WebApplicationContext: initialization completed in 616 ms
    2023-03-15T17:49:05.740-04:00  WARN 25057 --- [           main] ConfigServletWebServerApplicationContext : Exception encountered during context initialization - cancelling refresh attempt: org.springframework.beans.factory.UnsatisfiedDependencyException: Error creating bean with name 'dataSourceScriptDatabaseInitializer' defined in class path resource [org/springframework/boot/autoconfigure/sql/init/DataSourceInitializationConfiguration.class]: Unsatisfied dependency expressed through method 'dataSourceScriptDatabaseInitializer' parameter 0: Error creating bean with name 'dataSource' defined in class path resource [org/springframework/boot/autoconfigure/jdbc/DataSourceConfiguration$Hikari.class]: Failed to instantiate [com.zaxxer.hikari.HikariDataSource]: Factory method 'dataSource' threw exception with message: Failed to determine a suitable driver class
    2023-03-15T17:49:05.741-04:00  INFO 25057 --- [           main] o.apache.catalina.core.StandardService   : Stopping service [Tomcat]
    2023-03-15T17:49:05.754-04:00  INFO 25057 --- [           main] .s.b.a.l.ConditionEvaluationReportLogger : 

    Error starting ApplicationContext. To display the condition evaluation report re-run your application with 'debug' enabled.
    2023-03-15T17:49:05.761-04:00 ERROR 25057 --- [           main] o.s.b.d.LoggingFailureAnalysisReporter   : 

    ***************************
    APPLICATION FAILED TO START
    ***************************

    Description:

    Failed to configure a DataSource: 'url' attribute is not specified and no embedded datasource could be configured.

    Reason: Failed to determine a suitable driver class

    Action:

    Consider the following:
      If you want an embedded database (H2, HSQL or Derby), please put it on the classpath.
      If you have database settings to be loaded from a particular profile you may need to activate it (no profiles are currently active).


    FAILURE: Build failed with an exception.

    * What went wrong:
    Execution failed for task ':bootRun'.
    > Process 'command '/opt/eclipse-jee-2022-12-R-linux-gtk-x86_64/plugins/org.eclipse.justj.openjdk.hotspot.jre.full.linux.x86_64_17.0.5.v20221102-0933/jre/bin/java'' finished with non-zero exit value 1

    * Try:
    > Run with --stacktrace option to get the stack trace.
    > Run with --info or --debug option to get more log output.
    > Run with --scan to get full insights.

    * Get more help at https://help.gradle.org

    BUILD FAILED in 4s
    4 actionable tasks: 4 executed

    davidho@dphxps17:~/sbootprojs/prezsb304$ 
    davidho@dphxps17:~/sbootprojs/prezsb304$ ./gradlew tasks
    Starting a Gradle Daemon, 1 incompatible Daemon could not be reused, use --status for details

    > Task :tasks

    ------------------------------------------------------------
    Tasks runnable from root project 'prezsb304'
    ------------------------------------------------------------

    Application tasks
    -----------------
    bootRun - Runs this project as a Spring Boot application.

    Build tasks
    -----------
    assemble - Assembles the outputs of this project.
    bootBuildImage - Builds an OCI image of the application using the output of the bootJar task
    bootJar - Assembles an executable jar archive containing the main classes and their dependencies.
    build - Assembles and tests this project.
    buildDependents - Assembles and tests this project and all projects that depend on it.
    buildNeeded - Assembles and tests this project and all projects it depends on.
    classes - Assembles main classes.
    clean - Deletes the build directory.
    jar - Assembles a jar archive containing the main classes.
    resolveMainClassName - Resolves the name of the application's main class.
    testClasses - Assembles test classes.

    Build Setup tasks
    -----------------
    init - Initializes a new Gradle build.
    wrapper - Generates Gradle wrapper files.

    Documentation tasks
    -------------------
    javadoc - Generates Javadoc API documentation for the main source code.

    Help tasks
    ----------
    buildEnvironment - Displays all buildscript dependencies declared in root project 'prezsb304'.
    dependencies - Displays all dependencies declared in root project 'prezsb304'.
    dependencyInsight - Displays the insight into a specific dependency in root project 'prezsb304'.
    dependencyManagement - Displays the dependency management declared in root project 'prezsb304'.
    help - Displays a help message.
    javaToolchains - Displays the detected java toolchains.
    outgoingVariants - Displays the outgoing variants of root project 'prezsb304'.
    projects - Displays the sub-projects of root project 'prezsb304'.
    properties - Displays the properties of root project 'prezsb304'.
    resolvableConfigurations - Displays the configurations that can be resolved in root project 'prezsb304'.
    tasks - Displays the tasks runnable from root project 'prezsb304'.

    Verification tasks
    ------------------
    check - Runs all checks.
    test - Runs the test suite.

    Rules
    -----
    Pattern: clean<TaskName>: Cleans the output files of a task.
    Pattern: build<ConfigurationName>: Assembles the artifacts of a configuration.

    To see all tasks and more detail, run gradlew tasks --all

    To see more detail about a task, run gradlew help --task <task>

    BUILD SUCCESSFUL in 2s
    1 actionable task: 1 executed
    davidho@dphxps17:~/sbootprojs/prezsb304$ 


and here is some more information ...

