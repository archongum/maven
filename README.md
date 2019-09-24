# GitHub Maven Repository

## Usage

1. add in `~/.m2/settings.xml`

```xml
<settings>
    ...

    <servers>
        <server>
            <id>archongum-maven-read-only</id>
            <username>archongum</username>
            <password>b9b7ad59efeac9301f4c7cb9dd2668a597862935</password>
        </server>
    </servers>

    ...
</settings>
```

2. add in `pom.xml`

```xml
<project>
    ...

    <repositories>
        <repository>
            <id>archongum-maven-read-only</id>
            <name>archongum</name>
            <url>https://maven.pkg.github.com/archongum/maven</url>
        </repository>
    </repositories>

    ...
</project>
```

Note: both of `<id>` must be the same.

3. Now add dependencies in `pom.xml`.

