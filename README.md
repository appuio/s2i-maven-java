# S2I Builder with Maven and Java

A very simple S2I builder which builds Java applications with Maven.

The following environment vars can be used to configure the build:

| Name             | Default           | Description                         |
|------------------|-------------------|-------------------------------------|
| `MVN_GOALS`      | `clean package`   | Maven goals to execute              |
| `MVN_SKIP_TESTS` | `true`            | If tests should be skipped          |
| `MVN_OPTS`       | `None`            | Additional options handed to Maven  |

For Information about how those vars can be configured see the [official docs on
Build Strategy Options][1]

For a very similar S2I Java builder with some more options and flexibility, consider [fabric8io-images/s2i](https://github.com/fabric8io-images/s2i), AKA [fabric8/s2i-java on Docker Hub](https://hub.docker.com/r/fabric8/s2i-java/).
It [includes support for Gradle and Java 11 in addition to Maven and Java 8 as per this blog post](http://blog2.vorburger.ch/2018/11/s2i-with-java-11-gradle-builds-for.html).

[1]: https://docs.openshift.com/container-platform/3.7/dev_guide/builds/build_strategies.html#configuring-the-source-environment
