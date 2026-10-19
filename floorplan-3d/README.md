# floorplan-3d

## 项目名
**floorplan-3d**（户型装修设计）

## 介绍 / 能力
纯前端的**浏览器户型设计工作室**，整个应用就是一个 `index.html`，无需构建、打开即用。

- **2D 平面布置**：按 1:60/1:100 比例显示（mm），从家具库拖入 60+ 种家具家电，可移动/旋转/调尺寸、贴墙吸附，带测量工具、非承重墙拆改、图层开关。
- **3D 场景**：一键切到 Three.js，鸟瞰/斜视/俯视多视角，第一人称 WASD 漫游、可开门，全高墙/剖切墙切换、日照滑块、夜景灯光，2D/3D 家具实时同步。
- **方案统计**：自动算房间与套内面积，换地面材料并按 5% 损耗估造价，撤销/重做、本地保存、导出 PNG / 导入导出 JSON，中英界面。

- 分类：空间设计 ｜ 浏览器里的户型设计工作室
- 语言：原生 HTML/CSS/JS（2D 用 SVG，3D 用 Three.js r160）｜ 默认分支 master ｜ Star（快照）~2.5k ｜ License MIT

## 上手
```bash
git clone https://github.com/wy51ai/floorplan-3d
# 直接用浏览器打开 index.html，或：
python3 -m http.server 8000
```
> 3D 场景经 jsDelivr CDN 加载 Three.js，首次需联网。快捷键 `T` 切换 2D/3D，漫游用 WASD。

## 适用场景
户型布置演示、装修方案草稿、可交互看房原型。

## 来源链接
- 仓库：https://github.com/wy51ai/floorplan-3d
