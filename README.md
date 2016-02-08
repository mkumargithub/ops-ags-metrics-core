# ops-ags-metrics-core
added p90th Percentile functionality in this project

# Functionality added into Snapshot.java:
```java
    /**
     * Returns the value at the 90th percentile in the distribution.
     *
     * @return the value at the 90th percentile
     * added by mkumar
     */
    public double get90thPercentile() { return getValue(0.90); }

```

# Updated class file list:
- Snapshot
- ConsoleReporter
- CsvReporter
- JmxReporter
- Slf4jReporter

**_Test classes:_**
- ConsoleReporterTest
- CsvReporterTest
- JmxReporterTest
- Slf4jReporterTest
- UniformSnapshotTest

# MVN Build Status:
```log
[INFO] --- findbugs-maven-plugin:3.0.0:check (default) @ metrics-core ---
[INFO] BugInstance size is 0
[INFO] Error size is 0
[INFO] No errors/warnings found
[INFO] 
[INFO] --- maven-install-plugin:2.3.1:install (default-install) @ metrics-core ---
[INFO] Installing C:\Users\mkumar\IdeaProjects\metrics-core\target\metrics-core-4.0.0-OMNIFONE.jar to C:\Users\mkumar\.m2\repository\io\dropwizard\metrics\metrics-core\4.0.0-OMNIFONE\metrics-core-4.0.0-OMNIFONE.jar
[INFO] Installing C:\Users\mkumar\IdeaProjects\metrics-core\pom.xml to C:\Users\mkumar\.m2\repository\io\dropwizard\metrics\metrics-core\4.0.0-OMNIFONE\metrics-core-4.0.0-OMNIFONE.pom
[INFO] Installing C:\Users\mkumar\IdeaProjects\metrics-core\target\metrics-core-4.0.0-OMNIFONE-sources.jar to C:\Users\mkumar\.m2\repository\io\dropwizard\metrics\metrics-core\4.0.0-OMNIFONE\metrics-core-4.0.0-OMNIFONE-sources.jar
[INFO] Installing C:\Users\mkumar\IdeaProjects\metrics-core\target\metrics-core-4.0.0-OMNIFONE-javadoc.jar to C:\Users\mkumar\.m2\repository\io\dropwizard\metrics\metrics-core\4.0.0-OMNIFONE\metrics-core-4.0.0-OMNIFONE-javadoc.jar
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time: 32.168s
[INFO] Finished at: Thu Feb 04 11:07:11 GMT 2016
[INFO] Final Memory: 29M/243M
[INFO] ------------------------------------------------------------------------
```