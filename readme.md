# SalaryTracker

[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-blue.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)  ![Made by Wang Nan](https://img.shields.io/badge/Made%20by-Wang%20Nan-brightgreen)

一个**轻量化的个人工资记账工具**，用于记录每月工资发放明细。

纯前端单文件应用，**无需安装、无需后端、无需数据库**，所有数据保存在本地，隐私安全可控。

## 🚀 在线使用

* **正式版（无演示数据）**：[点击进入](https://salary.wangnan.net)

* **演示版（含示例数据）**：[点击进入](https://salary.wangnan.net?demo=1)

> 💡 也可以直接下载 [index.html](index.html) 到本地，用 Chrome / Edge 双击打开即可使用。

## ✨ 功能特性

1. 记录每月工资明细：基本工资、绩效奖金、年终奖、补贴等收入项
2. 自动计算五险一金与个税：输入税前收入，按可配置比例自动算出养老/医疗/失业/公积金/个税
3. 支持**自定义收入/扣除项目**：交通补贴、企业年金、工会费等新条目可随时添加
4. 收入类型标注：工资薪金 / 劳务报酬 / 稿酬所得 / 其他收入
5. 按时间段与项目类型统计总额，月度趋势图与收入构成明细可视化
6. 数据独立存储为 JSON 文件（Chrome/Edge 支持自动读写），或浏览器本地存储
7. 支持导出 / 导入 JSON 备份，换设备无缝迁移
8. 启动封面页 + 专属 Logo，界面现代简洁

## 📖 使用方法

1. 打开应用后，点击「新增工资记录」，选择日期与收入类型
2. 开启「自动计算」，输入基本工资后，社保/公积金/个税按设置中的比例自动填充
3. 若实际工资条与自动计算不一致，可手动修改各扣除项，核对实发工资
4. 在「设置」中可调整各项扣除比例、个税起征点、专项附加扣除，以及添加自定义项目
5. 建议在「数据存储」中关联一个本地 JSON 文件，修改将自动写入，防止数据丢失
6. 定期「导出 JSON」备份数据

## 🔧 技术说明

* 纯 HTML + CSS + JavaScript，单文件零依赖
* 数据格式：JSON，含记录明细（含唯一 `id`）、设置参数（扣除比例、自定义项目）
* 个税计算：工资薪金按七级超额累进税率表，劳务报酬 / 稿酬按对应规则

## ✅ Update 20260901

1. 新增启动封面页与专属 Logo（Base64 SVG，可作 favicon）
2. 新增自动计算公式：按设置比例核算五险一金与个税，收入类型细分
3. 新增自定义收入 / 扣除项目，删除项目时同步清理历史记录
4. 图表按月汇总展示，UI 全面优化（对齐、居中、布局统一）
5. 设置参数随数据文件一起保存与恢复

## 🧑‍💻 Version

**Created:** Wang Nan, 2026.08.31

**Contact:**

* [me@wangnan.net](mailto:me@wangnan.net)

---
## ⚖️ License

This work is licensed under the **[CC BY-NC-SA 4.0 License](https://creativecommons.org/licenses/by-nc-sa/4.0/)**.

You are free to use, share, and adapt the code for **non-commercial purposes**, provided that:

* You must give **appropriate credit**, provide **a link to this License**, and indicate if modifications were made. You may give credit in any reasonable way, but you must not do so in any way that suggests that the licensor endorses you or your use.
* You **distribute any modifications under the same license**.

&copy; 2026 Wang Nan. All rights reserved.
