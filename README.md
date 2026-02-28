# 续命工坊 · 膜蛤版 (Xuming Studio)

一个受 Universal Paperclips 启发的网页放置/点击游戏。核心目标是 `续命`：

- 初始每次点击续命 `+1 秒`
- 花费已有秒数购买升级
- 利用手动增幅、自动产能、全局倍率不断滚雪球

## Preview

![Gameplay Preview](./gameplay.png)

## Features

- 单文件前端实现（HTML + CSS + JS，无依赖）
- 点击续命与自动续命双循环
- 主题化升级路线（红衣男孩、香港记者、hawaii guitar、西方的华莱士、鸭嘴笔、三个表、基本法）
- 随里程碑推进的日志事件
- 本地存档与离线收益
- 后台标签页按真实时间结算自动增长

## Quick Start

1. 克隆仓库
2. 直接用浏览器打开 `index.html`

也可以用任意静态服务器启动（可选）：

```bash
python3 -m http.server 8080
```

然后访问 `http://localhost:8080`。

## Gameplay Loop

1. 点击主按钮累计可支配秒数
2. 购买升级提高手动效率、自动效率或全局倍率
3. 解锁更高成本升级，进入指数增长阶段

## Save Data

游戏进度保存在浏览器 `localStorage`：

- key: `moha-clicker-save-v1`
- 支持手动保存、自动保存、重开轮回

## Project Structure

- `index.html`: 游戏完整实现
- `gameplay.png`: README 预览图
- `README.md`: 项目说明

## Theme References

- https://en.wikipedia.org/wiki/Moha_(meme)
- https://en.wikipedia.org/wiki/Jiang_Zemin_Hong_Kong_journalist_incident
- https://en.wikipedia.org/wiki/Jiang_Zemin
- https://zh.wikipedia.org/wiki/%E9%B8%AD%E5%98%B4%E7%AC%94
- https://www.youtube.com/watch?v=MrUl7GMrKLM
