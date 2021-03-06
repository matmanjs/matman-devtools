# matman-devtools-extensions

Chrome devtools extensions for [matman](https://github.com/matmanjs/matman) 。

## 如何使用

- 安装扩展程序之后，打开开发者工具
- 它将出现在 `Elements` 面板中，与 `Styles` 平级，命名为 "matman" 的子面板。只要选择了元素，则该工具会有相应的变化（与调试样式的体验一致）
- 同时还会有一个 `matman-exec` 的页面，与 `Elements` 平级，在其中可以进行爬虫脚本的编辑与执行，执行结果将实时反馈（目前仅支持一个函数的情况）

## 开发调试

### 安装

1. 运行 `npm i` 命令；
2. 运行 `npm run build:install` 命令；
3. 打开 chrome 浏览器，访问 `chrome://extensions/` ；
4. 点击右上角的 "开发者模式"；
5. 点击 "加载已解压的扩展程序"，然后选择到本项目的 `build` 目录即可

### 更新

当改变了代码之后，在 `chrome://extensions/` 找到本程序，点击 "刷新" 的图标，然后再重新打开开发者工具。

> 有时候刷新了程序还不够，可能还需要刷新页面，尤其是有 content script 的场景；为了识别当时加载的时最新的代码，建议在某些地方输出不一样的标记，例如 panel ui 中，或者使用 `console.log` 输出不一样的标记。

## 更多资料

- https://developer.chrome.com/extensions/devtools
- http://www.cnblogs.com/liuxianan/p/chrome-plugin-develop.html#%E5%86%99%E5%9C%A8%E5%89%8D%E9%9D%A2
- [Publish in the Chrome Web Store](https://developer.chrome.com/webstore/publish)
- https://chrome.google.com/webstore/developer/dashboard?hl=zh-CN&gl=CN

