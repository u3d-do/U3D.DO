# U3D.DO

U3D_DO 是一个模块化、可扩展的 Unity 框架，旨在通过多个独立模块的组合，为开发者提供灵活、易用的工具集，以提升游戏开发效率。每个模块可以单独使用，也可以组合使用。所有模块以 `com.u3d_do.unity.` 为命名空间前缀。

## 模块列表

### 1. `com.u3d_do.core` (核心模块)

- **说明**: 该模块为框架的核心模块，包含基础的核心功能与定义。可以没有该模块，作为其他模块的基础依赖。

### 2. `com.u3d_do.unity.base` (基础模块)

- **说明**: 包含常用的基础插件和编辑器扩展，帮助简化开发过程。

### 3. `com.u3d_do.unity.utility` (工具模块)

- **说明**: 提供一系列常用的静态工具脚本，例如数学运算、字符串操作、时间管理等，提升开发效率。

### 4. `com.u3d_do.unity.res` (资源管理模块)

- **说明**: 依赖 Addressable 或者 AssetBundle 实现资源的加载和热更新，方便管理游戏中的动态资源。

### 5. `com.u3d_do.unity.hot` (脚本热更模块)

- **说明**: 基于 HybridCLR 实现的脚本热更新功能，支持游戏的运行时脚本更新，减少发布版本的频率。

### 6. `com.u3d_do.unity.net` (网络模块)

- **说明**: 提供 TCP、UDP 和 Protobuf 等通信协议的实现，用于处理游戏的网络通信。

### 7. `com.u3d_do.unity.web` (Web 模块)

- **说明**: 负责 HTTP 请求的封装处理，支持 RESTful API 的调用与服务器交互。

### 8. `com.u3d_do.unity.build` (自动化打包模块)

- **说明**: 包含一系列与项目打包相关的脚本和工具，帮助优化和简化 Unity 项目的打包流程。

### 9. `com.u3d_do.unity.prefs` (持久化模块)

- **说明**: 提供对持久化文件的管理，并支持文件加密功能，确保本地数据的安全性。

### 10. `com.u3d_do.unity.data` (配表数据模块)

- **说明**: 提供配置文件的读取与管理功能，支持 JSON、XML 等格式，帮助项目处理多样化的配置需求。

### 11. `com.u3d_do.unity.ui` (UI 模块)

- **说明**: 依赖 `com.u3d_do.unity.res` 和 `com.u3d_do.unity.hot`，提供 UI 相关的功能和控件，方便构建复杂的 UI 界面。

### 12. `com.u3d_do.unity.i18n` (国际化模块)

- **说明**: 依赖 `com.u3d_do.unity.config` 模块，提供多语言支持和管理功能，简化国际化开发。

## 使用说明

每个模块可以独立使用，但部分模块存在依赖关系。根据项目需求，您可以自由组合使用这些模块来构建您的项目。

1. **导入模块**：将所需的模块克隆或导入到您的 Unity 项目中。
2. **依赖关系**：请确保导入的模块符合其依赖关系，例如 `com.u3d_do.unity.ui` 依赖 `com.u3d_do.unity.res` 和 `com.u3d_do.unity.hot`。
3. **定制化**：根据项目需求，您可以定制每个模块的功能。

您也可以通过 issues 来提出您的问题，我们及时为您解答。

请不要提问「现成」问题，即那些简单搜一搜就能得到答案的，对经验和洞察力几乎没有要求的问题。 

详请参考《[提问的智慧](https://github.com/ryanhanwu/How-To-Ask-Questions-The-Smart-Way/blob/master/README-zh_CN.md)》


## 友情链接

- [QFramework](https://github.com/liangxiegame/QFramework) QFramework 是一套 渐进式 的 快速开发 框架。目标是作为无框架经验的公司、独立开发者、以及 Unity3D 初学者们的 第一套框架。框架内部积累了多个项目的在各个技术方向的解决方案。学习成本低，接入成本低，重构成本低，二次开发成本低，文档内容丰富(提供使用方式以及原理、开发文档)。

- [XAssets](https://github.com/xasset/xasset) xasset 提供了一种使用资源路径的简单的方式来加载资源，简化了Unity项目资源打包，更新，加载，和回收的作业流程。 ([@吉缘](https://github.com/mmdnb))

- [GameFramework](http://gameframework.cn/) 是一个基于 Unity 5.3+ 引擎的游戏框架，主要对游戏开发过程中常用模块进行了封装，很大程度地规范开发过程、加快开发速度并保证产品质量。（[@Ellan](https://github.com/EllanJiang)）

- [ET框架](https://github.com/egametang/ET) 是一个Unity3d客户端+C#分布式服务端框架。使用组件式开发，提供客户端热更，服务端热更功能，提供erlang式分布式消息机制（[@熊猫](https://github.com/egametang)）

- [华佗/HyBridCLR](https://github.com/focus-creative-games/hybridclr) 是一个特性完整、零成本、高性能、低内存的近乎完美的Unity全平台原生c#热更新解决方案。


## 贡献

欢迎对该框架的贡献！如果您有任何想法、反馈或建议，欢迎提交 Issue 或 Pull Request。

[![Stargazers over time](https://starchart.cc/tdouguo/KIT.svg)](https://starchart.cc/tdouguo/KIT)

---

## 鸣谢

感谢 [JetBrains](https://www.jetbrains.com/?from=real-url) 提供的 free JetBrains Open Source license

[![JetBrains-logo](https://i.loli.net/2020/10/03/E4h5FZmSfnGIgap.png)](https://www.jetbrains.com/?from=real-url)
