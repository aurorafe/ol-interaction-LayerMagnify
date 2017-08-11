# openlayers 扩展图层放大镜功能

[![Build Status](https://www.travis-ci.org/aurorafe/ol-interaction-LayerMagnify.svg?branch=master)](https://www.travis-ci.org/aurorafe/ol-interaction-LayerMagnify)
[![NPM](https://nodei.co/npm/ol-interaction-LayerMagnify.png?downloads=true&downloadRank=true&stars=true)](https://nodei.co/npm/ol-interaction-LayerMagnify/)

> 提供图层滤镜功能（参考openlayers官方[示例](https://openlayers.org/en/latest/examples/magnify.html)）

## build

> 重要: Github 仓库的 /dist 文件夹只有在新版本发布时才会更新。如果想要使用 Github 上最新的源码，你需要自己构建。

---

```bash
git clone https://github.com/aurorafe/ol-interaction-LayerMagnify.git
npm install
npm run dev
npm run build
```

## Use

> `ol.interaction.LayerMagnify(options)`

### CDN

```bash
https://unpkg.com/ol-interaction-layermagnify@1.0.0/dist/ol-interaction-LayerMagnify.min.js
https://unpkg.com/ol-interaction-layermagnify@1.0.0/dist/ol-interaction-LayerMagnify.js
```

### NPM

```bash
npm install ol-interaction-layermagnify --save
import 'ol-interaction-layermagnify'
```

## Examples

[![demo](https://raw.githubusercontent.com/aurorafe/ol-interaction-LayerMagnify/master/asset/demo.png)](https://codepen.io/sakitam-fdd/pen/OjgdRg)

其他示例请参看example文件夹

## options:

| key | type | desc |
| :--- | :--- | :---------- |
| `magnifyLayer` | `Object` | 放大镜中图层 |
| `radius` | `Number` | 滤镜半径，默认 ``75`` |
| `minRadius` | `Number` | 滤镜可调整最小半径，默认 ``25`` |
| `maxRadius` | `Number` | 滤镜可调整最大半径，默认 ``150`` |
| `lineWidth` | `Number` | 滤镜边框宽度，默认 ``5`` |
| `strokeStyle` | `String` | 滤镜默认边框颜色，默认 ``rgba(0, 0, 0, 0.5)`` |
| `zoomInKeyCode` | `Number` | 键盘控制滤镜放大对应的keyCode，默认为 ``38`` 方向上 |
| `zoomOutKeyCode` | `Number` | 键盘控制滤镜缩小对应的keyCode，默认为 ``40`` 方向下 |

## Extends

> `ol.interaction.Pointer`

#### Methods

##### `setMap(map)`

> 设置当前地图实例

###### Parameters:

| key | type | desc |
| :--- | :--- | :---------- |
| `map` | `ol.Map` | 地图实例 |

