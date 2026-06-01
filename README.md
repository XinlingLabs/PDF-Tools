# 📄 PDF Tools

![Python](https://img.shields.io/badge/Python-3.10+-blue)
![Platform](https://img.shields.io/badge/Platform-Windows-lightgrey)
![Status](https://img.shields.io/badge/Status-Stable-green)
![License](https://img.shields.io/badge/License-MIT-yellow)

一个基于 **Python + Tkinter + PyMuPDF + PyPDF** 的桌面 PDF 工具箱  
专为日常办公场景设计：拆分 / 重命名 / 校验 / 批量处理 / 可视化操作

---

## ✨ 核心能力

### 📌 1. PDF 规则拆分（自动切割）

输入：

3

效果：

1-3  
4-6  
7-9  

适用于：
- 批量报告拆分
- 固定页数分段导出

---

### 📌 2. 自定义拆分（灵活控制）

输入：

2,3,5

或：

2  
3  
5  

输出：

文件1：2页  
文件2：3页  
文件3：5页  

---

### 📌 3. 可视化拆分（核心功能 ⭐）

✔ PDF 缩略图预览  
✔ 点击放大查看  
✔ 勾选页面自动生成规则  

示例：

勾选：

1、3、6、10

自动生成：

1-3  
6-10  

特点：
- 适合不规则 PDF 拆分
- 可替代手动标页
- 提升 10x 操作效率

---

### 📌 4. 批量重命名

支持：

张三  
李四  
王五  

或：

张三,李四,王五  

适用于：
- 批量合同
- 批量报表
- 批量扫描件整理

---

### 📌 5. 交替命名（高级规则）

左侧：

A  
B  
C  

右侧：

1  
2  

输出：

A  
1  
B  
2  
C  

适用于：
- 双面文件
- 对照表结构文件
- 数据映射类文档

---

### 📌 6. 自动页数校验（防错误）

系统自动检测：

- 期望页数
- 实际页数

异常处理：

❌ 日志标红  
❌ UI 进度条变红  
❌ 弹窗提醒  

---

### 📌 7. CSV 结果导出

自动生成：

拆分结果.csv

内容包括：

- 文件名
- 期望页数
- 实际页数
- 校验状态

适用于：
- 审计
- 批量归档
- 自动化记录

---

### 📌 8. 拖拽支持（极简操作）

✔ 支持拖入 PDF  
✔ 支持多文件批处理  
✔ 自动识别模式  

---

### 📌 9. 输出目录管理

- 自动创建 output 文件夹
- 自动检测是否为空
- 支持清空 / 保留模式
- 防止误覆盖文件

---

## 🧠 技术架构

```text
UI层：Tkinter
PDF处理：PyPDF + PyMuPDF
拖拽支持：tkinterdnd2
并发处理：threading
