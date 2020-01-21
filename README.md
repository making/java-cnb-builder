# Cloud Native Buildpacks for Java

This builder uses lifecycle v0.5.0. So maake sure you are using `pack` v0.5.0 or later.

## Included Buildpacks
* [`openjdk-cnb`](https://github.com/cloudfoundry/openjdk-cnb)
* [`build-system-cnb`](https://github.com/cloudfoundry/build-system-cnb)
* [`jvm-application-cnb`](https://github.com/cloudfoundry/jvm-application-cnb)
* [`spring-boot-cnb`](https://github.com/cloudfoundry/spring-boot-cnb)
* [`procfile-cnb`](https://github.com/cloudfoundry/procfile-cnb)
* [`jvmkill-cnb`](https://github.com/making/jvmkill-cnb)
* [`memory-calculator-cnb`](https://github.com/making/memory-calculator-cnb)
* [`debug-cnb`](https://github.com/cloudfoundry/debug-cnb)
* [`jmx-cnb`](https://github.com/cloudfoundry/jmx-cnb)

## Build an image using this builder

```
pack build <image name> --builder making/java-cnb-builder --path <path-to-java-project-or-jar-file>
```

## Build a builder

```
pack create-builder -b builder.toml making/java-cnb-builder --publish
```

## License
This buildpack is released under version 2.0 of the [Apache License][a].

[a]: https://www.apache.org/licenses/LICENSE-2.0
