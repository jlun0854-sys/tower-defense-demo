# 🏰 Tower Defense Demo

基于流场寻路算法（Flow Field Pathfinding）的动态网格塔防游戏，支持实时堵路判定与防封路机制。

🎮 **[点击这里直接在线试玩游戏！](https://jlun0854-sys.github.io/tower-defense-demo/)**

---

## ✨ 核心特性

- **动态寻路系统**：采用 Flow Field 算法计算地图流场，支持大量怪物高效寻路。
- **智能建塔校验**：内置 `wouldBlock` 逻辑，在玩家放置/拆除防御塔时实时预演路径，防止怪物路径被彻底封死。
- **无缝状态恢复**：寻路校验采用污染隔离机制，在不更新/破坏全局渲染路径的前提下完成合法性判断。
- **网格交互**：支持鼠标悬停（Hover）实时预览建塔位置与路径状态。

## 🛠️ 技术栈

- **前端/渲染**：JavaScript (ES6+) / HTML5 Canvas
- **核心算法**：Flow Field (BFS / Dijkstra 算法延伸)
