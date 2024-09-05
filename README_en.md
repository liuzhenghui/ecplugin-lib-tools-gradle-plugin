# ecplugin-lib-tools-gradle-plugin

**[中文](README.md) | [English](README_en.md)**

- Analyze jar file information (pom) in the lib directory
- If the Maven repository does not exist, generate a Gradle module that can be pushed to the repository
- Compare the differences between two lib directory jar files

## Usage

```groovy
plugins {
    id 'ecplugin-lib-tools-gradle-plugin' version '<version>'
}
```

### List jar information

```bash
gradle libList
```

> The analysis result is generated as `build/reports/libs.html`

### Generate module based on jar

```bash
gradle libCreateModules
```

> The analysis results are generated as `build/reports/lib-modules.html`
> Generate Gradle project to `lib-modules/`

### Compare lib directories

```bash
gradle libDiff
```

> The analysis result is generated as `build/reports/lib-diff.html`