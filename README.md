# ecplugin-lib-tools-gradle-plugin

**[中文](README.md) | [English](README_en.md)**

- 解析 lib 目录下 jar 文件信息(pom)
- 若 maven 仓库不存在，生成 gradle 模块，可推送至仓库
- 比较两个 lib 目录 jar 文件差异

## 使用方法

```
plugins {
    id 'ecplugin-lib-tools-gradle-plugin' version '<version>'
}
```

### 列出 jar 信息

```bash
gradle libList
```

> 分析结果生成为 `build/reports/libs.html`

### 根据 jar 生成 module

```bash
gradle libCreateModules
```

> 分析结果生成为 `build/reports/lib-modules.html`
> gradle 工程生成到 `lib-modules/`

### 比较两个 lib 目录

```bash
gradle libDiff
```

> 分析结果生成为 `build/reports/lib-diff.html`
