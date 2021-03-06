---
title: Stable Version
---

 Setup Koin for your project 

### Current Version

Here are the current versions of Koin:

```groovy
// latest stable
koin_version = '2.2.2'
```

## Gradle 

### Jcenter 

Check that you have the `jcenter` repository. 

```groovy
// Add Jcenter to your repositories if needed
repositories {
	jcenter()    
}
```

### Dependencies

Pick one of your Koin dependency:

#### Gradle Plugin

```groovy
buildscript {
    repositories {
        jcenter()
    }
    dependencies {
        classpath "org.koin:koin-gradle-plugin:$koin_version"
    }
}

apply plugin: 'koin'
```

#### Core features

```groovy
// Koin for Kotlin
implementation "org.koin:koin-core:$koin_version"
// Koin extended & experimental features
implementation "org.koin:koin-core-ext:$koin_version"
// Koin for Unit tests
testImplementation "org.koin:koin-test:$koin_version"
// Koin for Java developers is now part of core
// implementation "org.koin:koin-java:$koin_version"
```

#### Android

```groovy
// Koin for Android
implementation "org.koin:koin-android:$koin_version"
// Koin Android Scope features
implementation "org.koin:koin-android-scope:$koin_version"
// Koin Android ViewModel features
implementation "org.koin:koin-android-viewmodel:$koin_version"
// Koin Android Experimental features
implementation "org.koin:koin-android-ext:$koin_version"
```

#### AndroidX

```groovy
// Koin AndroidX Scope features
implementation "org.koin:koin-androidx-scope:$koin_version"
// Koin AndroidX ViewModel features
implementation "org.koin:koin-androidx-viewmodel:$koin_version"
// Koin AndroidX Fragment features
implementation "org.koin:koin-androidx-fragment:$koin_version"
// Koin AndroidX WorkManager
implementation "org.koin:koin-androidx-workmanager:$koin_version"
// Koin AndroidX Jetpack Compose
implementation "org.koin:koin-androidx-compose:$koin_version"
// Koin AndroidX Experimental features
implementation "org.koin:koin-androidx-ext:$koin_version"
```

#### Ktor

```groovy
// Koin for Ktor Kotlin
implementation "org.koin:koin-ktor:$koin_version"
```