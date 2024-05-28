# OSS Parent

Open Source Software Maven parent POM. All Sentry Software's open-source Java projects must inherit this POM.

## Usage

You can use this parent POM by adding the following `parent` element to the beginning of your project's POM file

```xml
<parent>
    <groupId>org.sentrysoftware</groupId>
    <artifactId>oss-parent</artifactId>
    <version>${project.version}</version>
</parent>
```
