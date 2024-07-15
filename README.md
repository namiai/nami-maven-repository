# nami maven repository

#### Configure Repository

## In settings.gradle.kts (or settings.gradle) file, add nami maven repo url

```kotlin
dependencyResolutionManagement {
    repositoriesMode.set(RepositoriesMode.FAIL_ON_PROJECT_REPOS)
    repositories {
        google()
        mavenCentral()
        maven {
            name = "nami-maven-repository-releases"
            setUrl("https://raw.githubusercontent.com/namiai/nami-maven-repository/main/repository/releases")
        }
    }
}
```

## In build.gradle.kts ( or build.gradle) of your module, add nami-sdk-ui as your dependency.

```kotlin
dependencies {
    // existing dependencies

    // add this implementation
    implementation("ai.nami:sdk-ui:2.0.9")
    
}

```

## For using nami-sdk-routing or core-sdk check our SDK document for more detail
