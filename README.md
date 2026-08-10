# Literature Touch

推荐发布版本。

固定统计时段（UTC+8）：
- 08:00–12:00
- 14:00–17:00
- 19:00–23:00

设计规则：
- 当前小时未结束前不会提前算 missed。
- 同一小时可以多次“进入文献”，每次点击都会累计；小时格显示 ×1 / ×2 / ×3…。
- 新增“平均进入 / 有效小时”指标：今日累计进入次数 ÷ 今天已经开始且未被排除的有效小时数。
- 命中率只使用已经结束的有效小时。
- 固定休息时间不进入分母。
- 大块项目只能排除当前或未来小时，不允许事后洗掉 missed。
- missed 原因是可选回顾，不要求补偿。
- 不使用 streak 或硬性每日目标。
- 支持 JSON 导出和导入备份。

GitHub Pages：
1. 新建 repository（例如 literature-touch）。
2. 上传本目录中的 index.html、manifest.webmanifest、sw.js、icon-192.png、icon-512.png。
3. Settings → Pages → Deploy from a branch → main → /(root) → Save。
4. 用 Safari 打开 GitHub Pages 地址，再添加到主屏幕。
