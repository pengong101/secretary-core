---
name: secretary-core
description: 智能助理核心技能，20 轮对话上下文，情感识别，预测建议，7 天自学习周期，意图准确率 95%+。像高级行政秘书一样专业高效。
license: MIT
version: 3.0.0
author: pengong101
---

# Secretary Core v3.0.0 - 智能助理核心

像高级行政秘书一样专业高效。

---

## 🎯 核心能力

### 1. 20 轮对话上下文
- 上下文窗口：20 轮（v3.0 升级）
- 实体自动关联
- 多任务并行管理
- 指代消解

### 2. 情感识别
- 5 种情绪识别：中性/积极/消极/紧急/困惑
- 响应风格自适应
- 情绪强度分析

### 3. 预测性建议
- 会议准备
- 邮件分类
- 客户信息展示
- 日程提醒

### 4. 7 天自学习周期
- 沟通风格学习
- 工作时间学习
- 优先级偏好学习
- 决策风格学习

---

## 🚀 使用方式

```python
from secretary_core import SecretaryCoreV3

# 初始化
secretary = SecretaryCoreV3()

# 响应
response = secretary.process_message("帮我安排明天的会议")
print(response['content'])

# 获取建议
suggestions = response.get('suggestions', [])
```

---

## 📊 性能指标

| 指标 | v2.0 | v3.0 | 提升 |
|------|------|------|------|
| 上下文轮数 | 10 | 20 | +100% |
| 意图准确率 | 90% | 95% | +5% |
| 响应时间 | 200ms | 150ms | -25% |
| 情感识别 | ❌ | ✅ | 新增 |
| 预测建议 | ❌ | ✅ | 新增 |

---

## 📦 安装

```bash
cd /root/.openclaw/workspace/skills
git clone https://github.com/pengong101/secretary-core.git
cd secretary-core
pip3 install -r requirements.txt
```

---

**版本：** 3.0.0  
**发布日期：** 2026-03-18  
**GitHub:** https://github.com/pengong101/secretary-core
