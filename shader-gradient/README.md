# Shader Gradient

## 项目名
**shader-gradient**（Jannchie 版，框架无关重构）；上游原版 **ruucm/shadergradient**

## 介绍 / 能力
可定制的 **流动 Shader 渐变**。本仓库（Jannchie/shader-gradient）受 [`ruucm/shadergradient`](https://github.com/ruucm/shadergradient) 启发，把渲染引擎抽成框架无关的纯 TypeScript 核心，再提供 React / Vue 薄绑定，不必绑定 React。

- `@shader-gradient/core`：直接作用于 DOM + Three.js，框架无关
- `@shader-gradient/react` / `@shader-gradient/vue`：同一渲染器的薄绑定
- 共享预设、query-string 序列化、相机控制、HDR 环境、多种 shader 族（defaults / positionMix / cosmic / glass / lava / aurora / marble / pulse）与网格类型（plane / sphere / waterPlane）

- 分类：动态渐变
- 语言：TypeScript ｜ 默认分支 main ｜ Star（快照）~20（上游 ruucm 版 ~2.9k）

## 上手（Jannchie 版）
```bash
npm install @shader-gradient/core        # 框架无关
npm install @shader-gradient/react      # React 绑定
npm install @shader-gradient/vue         # Vue 绑定
```

```ts
import { ShaderGradient } from '@shader-gradient/core'

const gradient = new ShaderGradient(container, {
  preset: 'pensive',
  type: 'sphere',
  shader: 'defaults',
  lightType: 'env',
  envPreset: 'city',
})
```

## 上游原版（React 首选，生态最成熟）
ruucm/shadergradient：可在 Framer、Figma、React 中使用的 3D 流动渐变，在线定制器 https://www.shadergradient.co/customize 。

```bash
npm i @shadergradient/react @react-three/fiber three three-stdlib camera-controls
```

## 适用场景
品牌背景、Hero 动态底色、氛围渐变横幅。

## 来源链接
- 本仓库（按名收录）：https://github.com/Jannchie/shader-gradient
- 上游原版：https://github.com/ruucm/shadergradient
- 在线定制：https://www.shadergradient.co/customize
