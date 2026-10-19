# React Three Fiber

## 项目名
**@react-three/fiber**（react-three-fiber）

## 介绍 / 能力
Three.js 的 **React 渲染器（React renderer）**。用可复用、自包含的声明式 JSX 组件搭建 3D 场景，组件能响应状态、响应指针事件并参与 React 生态；JSX 里的 `<mesh />` 直接对应 `new THREE.Mesh()`，Three.js 新能力立即可用。渲染发生在 React 之外，无额外开销。

- 分类：3D 交互
- 语言：TypeScript ｜ 默认分支 master ｜ Star（快照）~33k ｜ License MIT
- 文档：https://docs.pmnd.rs/react-three-fiber

## 上手
```bash
npm install three @types/three @react-three/fiber
```
> 版本配对：`@react-three/fiber@8` 配 `react@18`，`@react-three/fiber@9` 配 `react@19`。

```jsx
import { Canvas, useFrame } from '@react-three/fiber'

<Canvas>
  <ambientLight intensity={Math.PI / 2} />
  <Box position={[-1.2, 0, 0]} />
  <Box position={[1.2, 0, 0]} />
</Canvas>
```

## 适用场景
可旋转/拖拽的 3D 产品展示、沉浸式 Hero 首屏、3D 数据可视化、互动原型。

## 来源链接
- 仓库：https://github.com/pmndrs/react-three-fiber
- 配套生态：[@react-three/drei](https://github.com/pmndrs/drei)（帮助函数）、[@react-three/postprocessing](https://github.com/pmndrs/react-postprocessing)（后期特效）、[@react-three/xr](https://github.com/pmndrs/react-xr)（VR/AR）
