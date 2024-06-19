# nami maven repository

#### Configure Repository

```kotlin
repositories {
    maven {
        name = "nami-maven-repository-releases"
        setUrl("https://raw.githubusercontent.com/namiai/nami-maven-repository/main/repository/releases")
    }
    maven {
        name = "nami-maven-repository-snapshots"
        setUrl("https://raw.githubusercontent.com/namiai/nami-maven-repository/main/repository/snapshots")
    }
}
```
