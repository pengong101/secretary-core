---
name: secretary-core
description: 智能助理核心技能，20 轮对话上下文，情感识别，预测建议，7 天自学习周期。
license: MIT
version: 3.0.0
author: pengong101
updated: 2026-03-18
---

# Secretary Core v3.0.0

**版本：** 3.0.0  
**更新日期：** 2026-03-18  
**作者：** pengong101  
**许可：** MIT

---

## 🎯 技能功能

### v3.0.0 核心能力

**1. 20 轮对话上下文**
- 上下文窗口：20 轮（v2.0 的 2 倍）
- 实体自动关联
- 指代消解

**2. 情感识别**
- 5 种情绪识别
- 响应风格自适应

**3. 预测性建议**
- 会议准备
- 邮件分类
- 日程提醒

**4. 7 天自学习周期**
- 沟通风格学习
- 工作时间学习

---

## 💻 使用方式

```python
from secretary_core import SecretaryCoreV3

# 初始化
secretary = SecretaryCoreV3()

# 响应消息
response = secretary.process_message("帮我安排明天的会议")
print(response['content'])

# 获取建议
suggestions = response.get('suggestions', [])
for s in suggestions:
    print(f"💡 {s}")

# 获取状态
status = secretary.get_status()
print(f"上下文轮数：{status['context_turns']}")
```

---

## 📊 版本历史

| 版本 | 日期 | 主要更新 |
|------|------|---------|
| **v3.0.0** | 2026-03-18 | 20 轮上下文、情感识别、预测建议 |
| v2.1.0 | 2026-03-14 | 自适应响应、性能优化 |
| v2.0.0 | 2026-03-13 | 10 轮上下文、主动预判 |
| v1.5.0 | 2026-03-12 | 多轮对话优化 |
| v1.0.0 | 2026-03-11 | 初始版本 |

---

## 📦 文件说明

```
secretary-core/
├── SKILL.md                  # 技能文档
├── README.md                 # 使用说明
├── LICENSE                   # MIT 许可证
├── clawhub.json              # ClawHub 配置
├── requirements.txt          # Python 依赖
├── secretary_v3.0.0.py       # v3.0.0 主程序
├── secretary_v2.1_adaptive.py # v2.1 版本
├── secretary_v2.py           # v2.0 版本
├── secretary_v1.5.py         # v1.5 版本
└── secretary_efficiency_v1.py # v1.0 版本
```

---

## 📈 性能指标

| 指标 | 数值 |
|------|------|
| 意图准确率 | 95%+ |
| 响应时间 | <150ms |
| 上下文轮数 | 20 轮 |
| 情感识别 | 5 种 |

---

**最后更新：** 2026-03-18  
**版本：** 3.0.0 (Latest)  
**许可：** MIT License
