---
title: TypeScript快速上手
date: 2018-09-17 22:36:53
tags:
    - 前端
    - JavaScript
---

TypeScript快速上手, 深入请看 [深入理解 TypeScript](https://jkchao.github.io/typescript-book-chinese/)

### 上手工具

工欲善其事必先利其器

1. [微软大杀器 VSCode](https://code.visualstudio.com/)
2. [Node环境](https://nodejs.org/zh-cn/)
3. Node环境模块: TypeScript, Ts-lint 和 ts-node，快速安装
> npm install -g typescript tslint ts-node
4. VSCode 插件：TSLint, Code Runner, TypeScript Hero, TypeScript Toolbox
5. 快速码字
> tsc --init
> tslint --init
> parcel 快速开发
> create-react-app new-app --scripts-version=react-scripts-ts
> 声明全局 global.d.ts
6. 使用ts来开发lib，推荐 [tsxd](https://github.com/palmerhq/tsdx)

### 使用技巧

1. 借助 VSCode 可以适当改下 `tslint` 规则
2. `window` 的全局方法要合理判断，如 `XMLHttpRequest` 方法需要 `if ((window as any).XMLHttpRequest)`, 因为IE下是 `ActiveXObject`