# Remotion 话术本

## 在 prompt-to-motion-graphics 里

> 启动：`npm run dev`，浏览器打开后输入提示词

### 常用提示词模板

**图表类**
```
做一个柱状图，数据是：产品A 120、产品B 85、产品C 200
蓝色柱子，从左到右依次出现，每个间隔0.3秒
```

**文字动画类**
```
标题"项目汇报"，大号白色字体，黑色背景
弹跳进入，持续2秒，带弹簧效果
```

**UI 模拟类**
```
做一个聊天界面，绿色气泡在右边，灰色气泡在左边
气泡有圆角，文字先显示右边再显示左边
```

**数据看板类**
```
做一个环形进度条，显示78%
蓝色渐变，数字在中间，从0开始动画增长
```

### 提示词原则

1. **颜色要说清楚** — "蓝色"、"黑金风格"、"冷色调"
2. **时间要说清楚** — "每个元素间隔0.3秒"、"持续2秒"
3. **动画感觉要说清楚** — "弹跳"、"平滑淡入"、"依次出现"
4. **数据直接写进去** — 不要"展示销售数据"，要"产品A 120、产品B 85"

## 在 prompt-to-video 里

> 启动：`npm run gen`，输入标题+主题

### 好用的主题
- 历史故事（"大禹治水的真相"）
- 冷知识（"为什么键盘是QWERTY排列"）
- 科普（"量子计算是什么"）

## 用那81个模板

模板路径：`F:\screen-recording-motion-essay\assets\remotion-templates\templates\`

### 按场景选模板

| 想做什么 | 用哪个模板 |
|----------|-----------|
| 片头标题 | `cinematic-title-intro.tsx` 或 `chapter-title.tsx` |
| 数据展示 | `chart-animation.tsx` 或 `bar-chart.tsx` 或 `pie-chart.tsx` |
| 图片展示 | `image-carousel.tsx` 或 `ken-burns.tsx` |
| 场景切换 | `cross-dissolve.tsx` 或 `slide-wipe.tsx` |
| 文字强调 | `bounce-text.tsx` 或 `glitch-text.tsx` |
| Logo 展示 | `logo-bounce-drop.tsx` 或 `logo-stroke-draw.tsx` |
| 片尾 | `end-card.tsx` 或 `credits-roll.tsx` |
| 背景氛围 | `bokeh-circles.tsx` 或 `gradient-shift.tsx` |
| 倒计时 | `countdown-intro.tsx` |

### 用法
直接复制 `.tsx` 文件到你的 Remotion 项目的 `src/` 里，然后在 `Root.tsx` 里注册 Composition 就能用。
