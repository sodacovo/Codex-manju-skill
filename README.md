# 🎬 Codex-manju-skill · AI 漫剧 SOP

> 小说选本评分 → 剧本改编 → 可视化转写 → 影视视角精修 → 剧本校验 → 人物/场景资产生成 → 分镜标注

一套面向 **竖屏短剧 / AI 漫剧** 全生命周期的工业级导演技能包，供 AI 助手 / LLM 直接调用。

完整规则库见 [`short-drama-director/`](short-drama-director/)

---

## 🎥 核心管线

```
📋 立项锁定 → ✍️ 五阶门控编剧 → 🎙️ 台词诊断 → 🖼️ 数字资产锁定 → 🎬 文武分镜 → 🚀 视频提示词渲染 → ✅ 独立质检
```

**核心理念：资产图先于分镜。** 角色/场景/道具在 P2 阶段完成**出图并锁定**，分镜和视频提示词一律引用已锁定的资产图，而非文字描述。

---

## ✨ 能做什么

| 场景 | 说明 |
|------|------|
| 小说 → 剧本 | 五阶门控改编（前提 → 结构 → 节拍 → 世界观 → 排版），拒绝无大纲直奔台词 |
| 台词优化 | 七维诊断 + 语速自检，杜绝播音腔，保障三档语速适配 |
| 资产出图 | A/B/C 分级锁定，角色亲缘遗传推导，直接生成人物/场景资产图 |
| 文戏分镜 | 微表情六阶段，对白保护，横竖屏自适应 |
| 武戏分镜 | 23 门武学 + 9 套剑法 + 11 环杀招，15s 完播率三档评分 |
| 玄幻战斗 | 法宝/五行术法/能量具象/对军清场，专为 R3 档设计 |
| 情绪曲线 | 12 节拍全片情绪张力量化，可视化绘图 |
| 视频提示词 | Seedance 2.5 三层解耦模板，16:9 / 9:16 全覆盖 |

---

## 📁 项目结构

```
Codex-manju-skill/
├── short-drama-director/           # V6.5 Multi-Agent 主包（39 文件）
│   ├── SKILL.md                    # 总控路由 + 指令清单
│   ├── references/                 # 33 个专业规则库 + 端到端总SOP
│   │   ├── end-to-end-manju-sop.md #   全流程 SOP（选本→成片）
│   │   ├── asset-first-pipeline.md #   Asset-First 六阶段
│   │   ├── seedance-render-engine.md # 渲染引擎
│   │   ├── combat-direction-engine.md # 武打导演
│   │   └── ... 共 33 模块
│   ├── scripts/
│   │   ├── check_package.py        # 静态自检
│   │   └── generate_emotion_curve.py # 情绪曲线绘图
│   ├── README.md / CHANGELOG.md / 使用说明.md
│   └── 截图/                       # 实际运行截图
│       ├── 小说1.0.png ~ 1.3.png   #   选本评分流程
│       └── 小说2.0 ~ 2.1.png       #   剧本改编流程
└── README.md
```

---

## 🚀 快速开始

```bash
# 安装到 OpenClaw
openclaw skills install ./short-drama-director --as short-drama-director

# 自检包完整性
python3 short-drama-director/scripts/check_package.py
```

完整使用说明：[`short-drama-director/使用说明.md`](short-drama-director/使用说明.md)

---

## 📜 版本历史

- **V6.5 Multi-Agent**（2026-09-02）— Asset-First 六阶段 + 多平台适配 + Seedance 2.5 深度适配
- **V6.0**（2026-08-28）— 23 模块重组 + 审计修复
- **V5.0.2**（2026-08-27）— 武学招式库补全

---

## 📄 License

MIT · 供创作学习使用，输出内容请自行遵守平台内容规范

---

<p align="center">
  <sub>📫 欢迎 Fork / Star，欢迎在 Issues 里与我讨论。</sub>
</p>
