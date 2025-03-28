# EFramework XMLHttpRequest for Unite

[![Version](https://img.shields.io/npm/v/org.eframework.uni.xhr)](https://www.npmjs.com/package/org.eframework.uni.xhr)
[![Downloads](https://img.shields.io/npm/dm/org.eframework.uni.xhr)](https://www.npmjs.com/package/org.eframework.uni.xhr)  

EFramework XMLHttpRequest for Unite 是一个基于 PuerTS 的 XMLHttpRequest 标准实现，可运行于 Unity、Unreal 等多个引擎环境中。

## 功能特性

- 🚀 跨平台：可运行于 Unity、Unreal 等多个引擎环境中
- 📦 标准兼容：完整实现 XMLHttpRequest Level 2 标准

### 核心功能

- Unity XMLHttpRequest：基于 UnityWebRequest 的 XMLHttpRequest 标准实现
- Unreal XMLHttpRequest：基于 Unreal HTTP 的 XMLHttpRequest 标准实现

### 平台支持

| Runtime/Platform | Windows | Linux | macOS | Android | iOS | Browser |
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| Node | ➖ | ➖ | ➖ | ➖ | ➖ | ➖ |
| Code | ➖ | ➖ | ➖ | ➖ | ➖ | ➖ |
| Cocos | ➖ | ➖ | ➖ | ➖ | ➖ | ➖ |
| Unity | ✅ | ✅ | ✅ | ✅ | ✅ | ➖ |
| Unreal | ❓ | ❓ | ❓ | ❓ | ❓ | ➖ |
| Electron | ➖ | ➖ | ➖ | ➖ | ➖ | ➖ |
| Dom | ➖ | ➖ | ➖ | ➖ | ➖ | ➖ |
- ✅已支持  ❓开发中  ❌未支持  ➖不适用

### 使用示例

```typescript
// Unity 环境
import { XMLHttpRequest } from "org.eframework.uni.xhr/unity"

const xhr = new XMLHttpRequest()
xhr.open("GET", "https://api.example.com/data")
xhr.onload = () => {
    console.log(xhr.response)
}
xhr.send()
```

## 常见问题

更多问题，请查阅[问题反馈](CONTRIBUTING.md#问题反馈)。

### 1. TypeScript 导入报错？
问题：Cannot find module 'org.eframework.uni.xhr/unity'
解决：将 tsconfig.json 的 moduleResolution 修改为 bundler 或 node16

## 项目信息

- [更新记录](CHANGELOG.md)
- [贡献指南](CONTRIBUTING.md)
- [许可证](LICENSE)
