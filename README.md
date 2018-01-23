# S2I Builder with Maven and Java

A very simple S2I builder which builds Java applications with Maven.

The following environment vars can be used to configure the build:

| Name             | Default           | Description                         |
|------------------|-------------------|-------------------------------------|
| `MVN_GOALS`      | `clean package`   | Maven goals to execute              |
| `MVN_SKIP_TESTS` | `true`            | If tests should be skipped          |
| `MVN_OPTS`       | `None`            | Additional options handed to Maven  |
