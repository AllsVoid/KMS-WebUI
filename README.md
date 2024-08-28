<p align="center"><img width="400" src="./src/assets/images/readme-logo.svg" /></p>

<p align="center">
<a href="https://github.com/ikxin/kms-tools/releases"><img src="https://badgen.net/github/release/ikxin/kms-tools" /></a>
<a href="https://github.com/ikxin/kms-tools/stargazers"><img src="https://badgen.net/github/stars/ikxin/kms-tools" /></a>
<a href="https://github.com/ikxin/kms-tools/network/members"><img src="https://badgen.net/github/forks/ikxin/kms-tools" /></a>
<a href="https://github.com/ikxin/kms-tools/commits"><img src="https://badgen.net/github/commits/ikxin/kms-tools" /></a>
<a href="https://github.com/ikxin/kms-tools/issues"><img src="https://badgen.net/github/issues/ikxin/kms-tools" /></a>
<a href="https://github.com/ikxin/kms-tools/watchers"><img src="https://badgen.net/github/watchers/ikxin/kms-tools" /></a>
<a href="https://github.com/ikxin/kms-tools/blob/master/LICENSE"><img src="https://badgen.net/github/license/ikxin/kms-tools" /></a>
</p>

## 📖 介绍

一站式 KMS 工具箱，集成了 KMS 激活脚本生成、KMS 服务器检测、KMS 服务器状态监控等功能。

该项目最早诞生于 2020 年 4 月，首发在 [Hostloc 论坛](https://hostloc.com/thread-669158-1-1.html)，之前仅仅只是一个用来生成 KMS 激活脚本的小工具。上大学的时候我在学校负责维护教学楼和机房的电脑设备，平日里经常需要重装各种各样版本的操作系统，这个小工具提高了激活操作系统的效率。于是在 2022 年 6 月，我将这个小工具翻出来，使用许多新技术对其进行了重构，再一次发布到了 [Hostloc 论坛](https://hostloc.com/thread-1026408-1-1.html)，得到了许多大佬的关注和支持。

后来的一段时间里也会偶尔更新一些功能，但一直都没有很完善，直到前些时候收到了两个特别的 issues「[#25](https://github.com/ikxin/kms-tools/issues/25)、[#26](https://github.com/ikxin/kms-tools/issues/26)」，其中有一个还是非中文语言发起的，我没有想到一个小小的项目能够得到海外朋友的关注。作为我开源的第一款「处女作」，我决定将其继续开发和维护下去。

原先的版本是一个纯前端的工具，为了实现 KMS 检测和 KMS 监控等功能，我使用 Bun + Elysia 写了一个后端服务，将整个项目区分为纯前端版本和全栈版本，前端版本可以调用 [kms.ikxin.com](https://kms.ikxin.com) 的 API 接口，而全栈版本则可以独立部署所有功能，甚至包含了 Vlmcsd 来作为 KMS 激活服务器。

## 📦 在线使用

### 全栈版本

- 官网地址: [kms.ikxin.com](https://kms.ikxin.com)

### 纯前端版本

- Cloudflare: [kmstools.pages.dev](https://kmstools.pages.dev)
- Vercel: [kmstools.vercel.app](https://kmstools.vercel.app)

## 👀 历史版本

|                                     |                                     |
| ----------------------------------- | ----------------------------------- |
| ![](./src/assets/images/v2.0.0.png) | ![](./src/assets/images/v1.2.0.png) |
| ![](./src/assets/images/v1.0.0.png) | ![](./src/assets/images/v0.1.5.png) |

## ✨ 技术栈

### 后端

- <img src="./src/assets/icons/logos/bun.svg" /> [Bun](https://github.com/oven-sh/bun) - 用于 JavaScript 和 TypeScript 应用程序的一体化工具包
- <img src="./src/assets/icons/logos/drizzle.svg" /> [Drizzle ORM](https://github.com/drizzle-team/drizzle-orm) - 下一代的无头 TypeScript ORM 框架
- <img src="./src/assets/icons/logos/elysia.svg" /> [Elysia](https://github.com/elysiajs/elysia) - 符合人体工程学的 Web 框架，用于使用 Bun 构建后端服务器

### 前端

- <img src="./src/assets/icons/logos/vue.svg" /> [Vue.js](https://github.com/vuejs/core) - 构建用户界面的 JavaScript 框架
- <img src="./src/assets/icons/logos/vite.svg" /> [Vite](https://github.com/vitejs/vite) - 下一代的前端工程构建工具
- <img src="./src/assets/icons/logos/arco.svg" /> [Arco Design Vue](https://github.com/arco-design/arco-design-vue) - ByteDance 开发的企业级产品设计系统
- <img src="./src/assets/icons/logos/vue-router.svg" /> [Vue Router](https://github.com/vuejs/vue-router) - Vue.js 核心团队开发的路由组件
- <img src="./src/assets/icons/logos/pinia.svg" /> [Pinia](https://github.com/vuejs/pinia) - 类型安全、可扩展性以及模块化设计的状态管理库
- <img src="./src/assets/icons/logos/vueuse.svg" /> [VueUse](https://github.com/vueuse/vueuse) - 基于 Composition API 的实用函数集合
- <img src="./src/assets/icons/logos/unocss.svg" /> [UnoCSS](https://github.com/unocss/unocss) - 即时的按需加载原子 CSS 引擎
- <img src="./src/assets/icons/logos/vue-i18n.svg" /> [Vue I18n](https://github.com/intlify/vue-i18n-next) - I18n 国际化支持
- <img src="./src/assets/icons/logos/unjs.svg" /> [unplugin-auto-import](https://github.com/antfu/unplugin-auto-import) - 自动按需导入 Composition API 的插件
- <img src="./src/assets/icons/logos/unjs.svg" /> [unplugin-vue-components](https://github.com/antfu/unplugin-vue-components) - 自动按需导入 Vue 组件的插件
- <img src="./src/assets/icons/logos/unjs.svg" /> [unplugin-vue-router](https://github.com/posva/unplugin-vue-router) - Vue Router 自动加载基于文件的路由系统
- <img src="./src/assets/icons/logos/markdown.svg" /> [unplugin-vue-markdown](https://github.com/unplugin/unplugin-vue-markdown) - Markdown 文档支持

## ⭐ 星星

<img src="https://starchart.cc/ikxin/kms-tools.svg" />

## 🧑‍💻 作者

Code with ❤️ by [一纸忘忧](https://www.ikxin.com '一纸忘忧')

## 📜 开源协议

[MIT License](./LICENSE 'MIT License')

Copyright (c) 2022~Present
