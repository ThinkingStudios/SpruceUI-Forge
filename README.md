<p align="center">
 <img width="100px" src="src/main/resources/icon.png" align="center" alt="SpruceUI-Forge port(Unofficial) Logo" />
 <h2 align="center">SpruceUI-Forge port (Unofficial)</h2>
 <p align="center">A Minecraft mod API which adds some GUI utilities.</p>
 <p align="center">
    <a title="Java 16" target="_blank"><img src="https://img.shields.io/badge/language-Java%2016-9B599A.svg?style=flat-square"></a>
    <a title="GitHub license" target="_blank" href="https://github.com/TexTrueStudio/SpruceUI/blob/ef21df009c38b34435a1b8e91c9b7a17f27cd5c3/LICENSE"><img src="https://img.shields.io/github/license/LambdAurora/SpruceUI?style=flat-square"></a>
    <a title="Environment: Client" target="_blank"><img src="https://img.shields.io/badge/environment-client-1976d2?style=flat-square"></a>
    <a title="Mod loader: Forge" target="_blank"><img src="https://img.shields.io/badge/Modloader-Forge-blue?style=flat-square"></a>
</p>

[简体中文](README_cn.md)

## Build

Just do `./gradlew build` and everything should build just fine!

## Use inside a mod

You can look at the [SpruceUI test mod](https://github.com/LambdAurora/SpruceUI/tree/1.16/src/testmod) for examples of use.

### Import inside a project

Add this to your `build.gradle` in addition of the base Fabric mod `build.gradle`:

```groovy
repositories {
    mavenLocal()
    maven { url 'https://jitpack.io' }
}

dependencies {
    modImplementation "com.github.TexTrueStudio:SpruceUI-Forge:${project.spruceui_version}"
}
```

And this to your `gradle.properties`:

```properties
spruceui_version=mc1.17-v0.1.0
```

It will JAR-in-JAR SpruceUI so users of your mod don't need to download it separately!
