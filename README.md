# 剧本资产表生成 Skill

> 🎬 一键将剧本解析为结构化资产表 | 自动生成带状态追踪和颜色标记的 Excel | Marvis 桌面助手专属 Skill

[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)
[![Stars](https://gitee.com/white-clad-er-zhuzi/script-asset-tool/badge/star.svg)](https://gitee.com/white-clad-er-zhuzi/script-asset-tool)

---

## 🤔 为什么需要这个工具

短剧/网文编剧在交付甲方前，需要整理一份**资产清单**——所有场景、人物、道具，标注出现集数、用途、外貌。一份 20 集的剧本，手搓资产表至少半天。

这个 Skill 把流程压缩到 **3 分钟**：丢剧本进去，Excel 自动生成，状态列带下拉菜单和颜色标记。

---

## 📊 输出效果

生成的 Excel 包含三个分表，五列结构：

| 资产名 | 完成状态 | 出现集数/场次 | 用途描述 | 外貌描写 |
|--------|:--------:|--------------|----------|----------|
| 中央医院 | 🔴未完成 | 第17集 第1场 | 丽贝卡急救抢救场景 | 白色走廊，急救设备齐全 |
| 丽贝卡 | 🟢已完成 | 第17-24集 | 女主角，悔悟赎罪主线 | 30岁，金发，憔悴但坚毅 |
| 遗嘱文件 | 🟡正在完成 | 第18集 第3场 | 维克多的秘密遗嘱道具 | 牛皮纸信封，火漆封印 |

**四种状态颜色实时切换：**
- 🔴 未完成 → 浅红底
- 🟢 已完成 → 浅绿底  
- 🟡 正在完成 → 浅黄底
- ⚪ 暂缓 → 灰底

---

## 🚀 使用方法

1. 将 `剧本资产表生成流程.md` 部署到 Marvis 桌面助手
2. 发送剧本文件 + 指令：

```
按资产表流程，处理这份剧本，第1集到最后
```

支持输入格式：**PDF / Word / Excel**，支持指定集数范围。

---

## 📁 文件结构

```
├── 剧本资产表生成流程.md    # Skill 核心文档（Excel 生成规范）
├── README.md                 # 本文件
└── LICENSE                   # MIT 开源协议
```

---

## 🎯 适用场景

- 📺 短剧制作流程中的资产梳理
- 📋 交付甲方前的资产清单整理  
- 🎥 剧组前期筹备的分工清单
- 🎨 美术/道具组的场景-道具对照表

---

## 🛠 技术要点

- 使用 openpyxl 生成 Excel
- CellIsRule 实现条件格式（仅填充色，字体不变）
- DataValidation 实现下拉菜单
- 深蓝底白字表头 + 冻结首行

---

## 📣 关于 Marvis

本 Skill 运行于 [Marvis 桌面助手](https://marvis.tencent.com)，一个支持 Windows 本地 AI 操作的工作台。

---

## ⭐ Star History

如果你觉得有用，点个 Star 支持一下～

[![Star History Chart](https://api.star-history.com/svg?repos=white-clad-er-zhuzi/script-asset-tool&type=Date)](https://star-history.com/#white-clad-er-zhuzi/script-asset-tool&Date)
