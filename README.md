# SachengTime

一个极简风格的世界时钟锁屏应用。

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

## 预览

SachengTime 是一款专为桌面设计的全屏时钟应用，融合世界时间、实时天气与今日进度追踪功能。采用无干扰的极简界面设计，适合作为电脑锁屏、待机画面或专注工作时的背景时钟。

## 功能特性

- **世界时钟** - 支持全球任意城市，自动处理时区转换
- **实时天气** - 显示当前城市天气状况与温度（数据来源：Open-Meteo）
- **今日进度** - 以百分比形式直观展示当天剩余时间
- **四色主题** - 默认黑 / 纯白 / 霓虹绿 / 复古琥珀，一键切换
- **防烧屏保护** - 智能微动算法，防止 OLED 屏幕烧屏
- **本地存储** - 自动记住你的城市设置
- **全屏模式** - 沉浸式全屏体验

## 快速开始

### 在线使用

直接访问：https://sachengsec.github.io/SachengTime/

### 本地运行

1. 克隆仓库
```bash
git clone https://github.com/sachengsec/SachengTime.git
```

2. 进入项目目录
```bash
cd SachengTime
```

3. 用浏览器打开 `index.html` 文件

或者使用本地服务器：

```bash
# Python 3
python -m http.server 8080

# Node.js
npx serve
```

然后访问 http://localhost:8080

## 使用指南

| 操作 | 说明 |
|------|------|
| 点击时钟 | 切换主题颜色 |
| 点击 ⚙️ 按钮 | 打开设置，切换城市 |
| 点击 ⛶ 全屏 | 进入/退出全屏模式 |
| 点击 🎨 切换主题 | 切换配色方案 |

### 切换城市

1. 点击右下角的 ⚙️ 设置按钮
2. 输入城市名称（支持中文，如：上海、纽约、东京）
3. 点击确认切换

## 主题展示

| 主题 | 描述 |
|------|------|
| 默认 | 黑色背景 + 白色文字 |
| 纯白 | 白色背景 + 黑色文字 |
| 霓虹 | 深绿背景 + 荧光绿文字，带发光效果 |
| 复古 | 棕色背景 + 琥珀色文字，带发光效果 |

## 技术栈

- 纯 HTML5 / CSS3 / JavaScript，零依赖
- 调用 [Open-Meteo API](https://open-meteo.com/) 获取天气与地理数据
- 使用 CSS 变量实现主题切换
- localStorage 持久化用户配置

## 浏览器支持

- Chrome / Edge / Firefox / Safari 最新版
- 支持 PWA，可安装为桌面应用

## 数据来源

- **天气数据**: [Open-Meteo](https://open-meteo.com/)（免费，无需 API Key）
- **地理编码**: [Open-Meteo Geocoding API](https://open-meteo.com/en/docs/geocoding-api)

## 项目结构

```
SachengTime/
├── index.html          # 主文件（包含 HTML + CSS + JS）
├── README.md           # 项目说明
└── LICENSE             # MIT 许可证
```

## 自定义字体（可选）

项目默认使用 Arial Black 作为 fallback 字体。如需使用自定义字体，请修改 CSS 中的 `@font-face` 部分：

```css
@font-face {
    font-family: 'TimeTravelerPalCustom';
    src: url('your-font-file.ttf') format('truetype');
}
```

## 开源协议

[MIT License](LICENSE)

## 致谢

- 天气数据由 [Open-Meteo](https://open-meteo.com/) 提供
- 灵感源自极简主义时钟设计

---

Made with ❤️ by [sachengsec](https://github.com/sachengsec)
