# 南山置业图鉴 · Nanshan Property Atlas

> 深圳南山豪宅的 AI 决策工具。进门选「买家 / 经纪」双模式：买家自助看房 + AI 选房；经纪陪客户谈（画像 + 对比 + AI 出话术）。

**🔗 在线 Demo：** https://nieears-cell.github.io/nanshan-atlas/

## 它解决什么
深圳 80% 的标志性豪宅在南山。买家与经纪面对的是信息分散、不直观、决策焦虑。本工具把"看懂南山 19 个核心豪宅"压缩到一屏、一句话。

## 三大能力
- 🤖 **真 AI 选房顾问**（Google Gemini）：自然语言需求 → 多约束**非线性权衡**（命中 ✓ / 让步 △ + 整体取舍）+ 经纪**带看话术**。用 `responseSchema` + 闭集 enum 防幻觉。
- 🏔 **3D 山海格局**（Cesium）：真实地形 + 高清卫星 + 立体楼块 + 山海地标，还原豪宅最核心的"背山面海"格局（含 GCJ-02→WGS-84 火星坐标纠偏）。
- 📊 **客观评分**：教育=距最近名校、医疗=距三甲…**实测距离换算**，事实层 / 判断层分离，每个分都可溯源。

## 技术栈
高德 JS API 2.0（2D）· Cesium 1.142（3D）· Turf.js（测距）· ECharts · GSAP · Gemini REST。单文件 HTML、零构建、CDN 加载、全程优雅降级。

## 使用
AI 功能需访问者**自带 Gemini API key**（仅存浏览器 localStorage，不上传、不入库）。点右下「✦ AI 选房顾问」→ ⚙ 设置 key。在 https://aistudio.google.com/apikey 免费获取。

## 说明
评分为基于公开资料与实测距离的综合评估，仅供参考，不构成投资建议。地图 token 已配域名白名单。

---
*Built with Claude Code · 经 OpenAI Codex 跨模型互审 + 修复 · 配套 PRD / 架构 / 质检文档（私有）。*
