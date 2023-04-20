# Prism4jX

Provide a grammar locator to create a Prism4j instance for other projects, just for my own use.

```java
final Prism4j prism4j = new Prism4j(new Prism4jGrammarLocator());
```

## Prerequisites

Add the JitPack repository to your build file.

Add it in your settings.gradle at the end of repositories:

```groovy
dependencyResolutionManagement {
    repositories {
        ...
        maven { url 'https://jitpack.io' }
    }
}
```

## Dependency

Add this to your module's `build.gradle` file.

```groovy
dependencies {
    implementation 'com.github.linhao1998:Prism4jX:1.0.0'
}
```

## Usage

Either use the `Prism4jGrammarLocator` provided by this library (`com.linhaodev.prism4jx.Prism4jGrammarLocator`) during construction of your `Prism4j` object, or create a new one and add all the languages you want from this library found under the `com.linhaodev.prism4jx.languages` package.