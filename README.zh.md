# Lenormand JSON

[English](README.en.md) | [简体中文](README.md)

[![GitHub release](https://img.shields.io/github/v/release/KevinGuo1007/lenormand-json?include_prereleases&sort=semver)](https://github.com/KevinGuo1007/lenormand-json/releases)
[![License](https://img.shields.io/github/license/KevinGuo1007/lenormand-json)](LICENSE)

一份包含 36 张雷诺曼卡牌基础信息的 JSON 数据集，并附带公共领域卡牌图片。

## 文件

- `lenormand.json`：卡牌基础数据
- `lenormand-images.json`：卡牌基础数据 + 图片路径
- `cards/`：36 张卡牌图片

## 快速使用

```js
const data = require("./lenormand-images.json");

console.log(data.cards[0]);
```

输出示例：

```json
{
  "name": "Rider",
  "number": "1",
  "playing_card": "9 of Hearts",
  "suit": "Hearts",
  "img": "cards/01-Rider.png"
}
```

## 数据来源

卡牌图片来自 Wikimedia Commons：
[*Das Spiel der Hofnung (The Game of Hope)*](https://commons.wikimedia.org/wiki/File:Das_Spiel_der_Hofnung_(The_Game_of_Hope).png)。

原始作品由 Johann Kaspar Hechtel 创作，时间为 1799 年。Wikimedia Commons 将该图片标记为 public domain。

## 许可

本项目中的 JSON 数据和文档使用 [MIT License](LICENSE)。

原始卡牌图像为 public domain。
