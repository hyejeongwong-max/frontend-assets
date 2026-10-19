# Liquid Glass JS

## 项目名
**liquid-glass-js**

## 介绍 / 能力
Apple Liquid Glass 风格的 **WebGL 玻璃效果库**，带来实时折射（refraction）、模糊（blur）与遮罩（masking）。支持三种形状：圆角矩形、正圆、胶囊/药丸；提供嵌套玻璃系统（子元素采样父容器输出）、实时参数调节、响应式与可定制着色。纯原生 JavaScript、无构建步骤，除页面采样用的 html2canvas 外零依赖。

- 分类：液态玻璃
- 语言：JavaScript ｜ 默认分支 main ｜ Star（快照）~1.5k ｜ License MIT
- 在线 Demo：https://dashersw.github.io/liquid-glass-js/

## 上手
无构建，直接引入脚本即可：

```html
<script src="https://cdn.jsdelivr.net/npm/html2canvas@1.4.1/dist/html2canvas.min.js"></script>
<script src="container.js"></script>
<script src="button.js"></script>
<script>
  const button = new Button({
    text: 'Click Me!',
    size: 32,
    type: 'rounded', // rounded | circle | pill
    onClick: () => alert('Hello Glass!')
  })
  document.body.appendChild(button.element)
</script>
```

核心类：`Container`（玻璃容器，可 `addChild` 嵌套）、`Button`（继承 Container，带文字与点击）。可调参数包括边缘强度、轮廓光、中心畸变、模糊半径、着色不透明度等。

## 适用场景
玻璃拟态按钮、导航栏、悬浮控件、仪表盘卡片。

## 来源链接
- 仓库：https://github.com/dashersw/liquid-glass-js
- Demo：https://dashersw.github.io/liquid-glass-js/
