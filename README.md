# OSS Parent

![License](https://img.shields.io/github/license/sentrysoftware/oss-parent)

Open Source Software Maven parent POM. All Sentry Software's open-source Java projects must inherit this POM.

## Build instructions

This project is a POM project. Nothing to build.

To install locally, run with:

```bash
mvn install
```

## Integrate in your project

You can use this parent POM by adding the following `parent` element to the beginning of your project's POM file:

```xml
<parent>
    <groupId>org.sentrysoftware</groupId>
    <artifactId>oss-parent</artifactId>
    <version>3</version>
</parent>
```

## Release instructions

The artifact is deployed to Sonatype's [Maven Central](https://central.sonatype.com/).

Use [GitHub Actions "Release to Maven Central"](actions/workflows/release.yml) to perform a release:

* Manually trigger the "Release" workflow
* Specify the version being released and the next version number (SNAPSHOT)
* Release the corresponding staging repository on [Sonatype's Nexus server](https://s01.oss.sonatype.org/)
* Merge the PR that has been created to prepare the next version

## License

License is Apache-2. Each source file must include the Apache-2 header (build will fail otherwise).
To update source files with the proper header, simply execute the below command:
