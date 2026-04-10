# Civil SBTI Starter v5

一个参照 SBTI Wiki 展示方式、但内容完全原创的「土木人专属人格测试」静态站点 starter。

## v5 这次重点修了什么

这版是针对“为什么老是测出来是 SAFE · 安全余量怪”做的平衡性修正版：

1. **把 SAFE 改得更尖**
   - SAFE 不再是一个全中间值人格
   - 强化了它在「规范依赖度 / 风险姿态 / 决策速度 / 关注焦点」上的特征

2. **降低聚合后掉回 M 的概率**
   - 聚合逻辑从简单平均取中间，改成更偏“多数派决定”
   - 两题同维度时：L+M 会判成 L，H+M 会判成 H，只有 L+H 才回到 M

3. **题目改得更逼人站队**
   - 选项不再只是“保守 / 中间 / 激进”弱区分
   - 改成更像三种不同人设在说话
   - 增加土木群聊黑话、甲方扯皮、AI、scope 锅、入行动机等场景

## 目录结构

```text
civil-sbti-starter-v5/
├── README.md
├── docs/
│   └── product-notes.md
└── web/
    ├── index.html
    ├── quiz.html
    └── data/
        ├── dimensions.json
        ├── outcomes.json
        └── questions.json
```

## 本地运行

推荐：VS Code + Live Server

1. 用 VS Code 打开整个文件夹
2. 安装 **Live Server**
3. 右键 `web/index.html` → `Open with Live Server`

## 你最常改的地方

- `web/data/questions.json`：题目
- `web/data/outcomes.json`：人格设定
- `web/index.html`：图鉴页
- `web/quiz.html`：独立测试页

## 备注

如果你后续要部署到 GitHub Pages，建议把 `web/` 里的内容移动到仓库根目录，或者放到 `/docs` 目录作为发布源。
