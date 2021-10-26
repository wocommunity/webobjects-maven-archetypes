![Master Build](https://github.com/wocommunity/webobjects-maven-archetypes/workflows/Master%20Build/badge.svg)

# WebObjects Maven Archetypes

Set of Maven archetypes to create WebObjects-related projects.

## Installation

### Command Line

Add the WOCommunity repository to your `~/.m2/settings.xml` file.

```xml
<profiles>
    <profile>
        <id>wocommunity</id>
        <activation>
            <activeByDefault>true</activeByDefault>
        </activation>
        <repositories>
            <repository>
                <id>wocommunity</id>
                <url>https://maven.wocommunity.org/content/groups/public/</url>
                <releases>
                    <enabled>true</enabled>
                </releases>
                <snapshots>
                    <enabled>true</enabled>
                </snapshots>
            </repository>
        </repositories>
    </profile>
</profiles>
```

\* **This step is not required if you use a repository manager that already points to the WOCommunity repository.**

### Eclipse

1. Open the Eclipse preferences.
2. Navigate to Maven > Archetypes section.
3. Click Add Remote Catalog...
4. Enter the catalog URL and description.
    - Catalog File: https://maven.wocommunity.org/content/groups/public/archetype-catalog.xml
    - Description: WOCommunity Catalog

## Usage

### Command Line

Run the archetype generate goal to create a new WebObjects project from the command line using Maven:

```shell
$ mvn archetype:generate -Dfilter=org.wocommunity:
```

### Eclipse

1. Create a new project using the Eclipse wizard.
2. Select the `Maven Project` option.
3. Select the WOCommunity Catalog from the catalog list.
4. Choose the catalog according to the project type.
5. Fill in the project information and finish.

## Contributing
Pull requests are welcome. For significant changes, please open an issue first to discuss what you would like to change.

## License
[Apache 2](https://www.apache.org/licenses/LICENSE-2.0.txt)