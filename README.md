# 📱 iPad 3 复古仪表盘 (Legacy iPad Dashboard)

> 让闲置的旧 iPad (iOS 9) 变身为精美的桌面时钟、日历与气象站。

本项目是一个纯静态的 HTML/JS 网页，专为 **iPad 3 / iPad 4 / iPad Mini 1** 等搭载 **iOS 9** 系统的老旧设备设计。它充分利用了 Retina 视网膜屏幕和 4:3 的屏幕比例，提供极致流畅的全屏体验。

![Dashboard Preview](https://via.placeholder.com/800x600?text=Dashboard+Preview)
*(建议在此处替换为您实际部署后的截图)*

## ✨ 核心特性

*   **⚡️ 极致兼容**：纯原生 HTML5/CSS3/ES5 JavaScript 编写，无现代框架依赖，iOS 9 Safari 秒开。
*   **📐 完美布局**：专为 1024x768 (4:3) 分辨率设计，左侧信息流，右侧超大日历。
*   **🌦 专业气象**：
    *   集成 **Open-Meteo** 免费 API（**无需 API Key**）。
    *   实时显示：**温度、相对湿度、空气质量 (AQI)、风速风向、紫外线强度 (UV)**。
    *   数据直接通过 JS 请求，无需加载外部图片或 iframe，稳定且节省流量。
*   **📅 智能日历**：本地 JS 生成万年历，支持中文年月显示，自动高亮“今天”和“周末”。
*   **📺 全屏模式**：支持 iOS Web App 标准，添加到主屏幕后隐藏地址栏，沉浸式显示。

## 🛠️ 配置说明 (修改城市)

默认坐标设置为 **中国·天津**。如果您需要修改为其他城市，请编辑 `index.html` 文件：

1.  打开 `index.html`。
2.  搜索代码块中的 `配置：天津坐标`。
3.  修改 `LAT` (纬度) 和 `LON` (经度) 变量。

```javascript
// --- 配置：您的城市坐标 ---
// 可以通过 Google Maps 或 OpenStreetMap 查询经纬度
var LAT = 39.14; // 纬度 (Latitude)
var LON = 117.20; // 经度 (Longitude)
