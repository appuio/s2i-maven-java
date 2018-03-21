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

[1]: https://docs.openshift.com/container-platform/3.7/dev_guide/builds/build_strategies.html#configuring-the-source-environment
