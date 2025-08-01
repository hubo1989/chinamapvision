# 中国地图可视化工具 (China Map Visualization Tool)

一个基于SVG的中国地图可视化数据生成工具，支持省份数据展示、颜色映射、交互式操作等功能。

## 功能特性

- 🗺️ **完整的中国地图** - 包含所有省份、自治区、直辖市和特别行政区
- 🎨 **数据可视化** - 支持数值数据的颜色映射和可视化展示
- 🖱️ **交互式操作** - 鼠标悬停显示详情、点击选择省份
- 🔍 **缩放和拖拽** - 支持地图缩放和拖拽操作
- 📊 **多种数据格式** - 支持简单数值和扩展格式数据输入
- 🎯 **精确定位** - 显示鼠标坐标和地理坐标信息
- 🏷️ **智能标签** - 自动隐藏无数据省份的标签
- 🎨 **自定义样式** - 支持颜色自定义和样式调整

## 在线演示

访问 [GitHub Pages](https://hubo1989.github.io/chinamapvision/) 查看在线演示。

## 本地运行

1. 克隆仓库：
```bash
git clone https://github.com/hubo1989/chinamapvision.git
cd chinamapvision
```

2. 启动本地服务器：
```bash
# 使用Python
python3 -m http.server 8080

# 或使用Node.js
npx serve .
```

3. 在浏览器中访问：
```
http://localhost:8080
```

## 使用方法

### 数据输入格式

#### 简单格式
```
北京,100
上海,200
广东,300
```

#### 扩展格式
```
北京,100,#ff0000,这是北京的数据
上海,200,#00ff00,这是上海的数据
广东,300,#0000ff,这是广东的数据
```

### 操作说明

1. **数据输入** - 在左侧面板输入省份数据
2. **颜色设置** - 选择最小值和最大值对应的颜色
3. **地图交互** - 鼠标悬停查看详情，点击选择省份
4. **缩放控制** - 使用缩放滑块或按钮调整地图大小
5. **拖拽移动** - 按住鼠标拖拽移动地图位置

## 技术特性

- **纯前端实现** - 无需后端服务器，可直接部署到静态网站
- **SVG渲染** - 矢量图形，支持无损缩放
- **响应式设计** - 适配不同屏幕尺寸
- **现代浏览器支持** - 兼容Chrome、Firefox、Safari、Edge等主流浏览器

## 文件结构

```
.
├── index.html              # 主页面文件
├── china-geojson/          # 中国地图GeoJSON数据
│   ├── china.json         # 主要地图数据
│   ├── geometryProvince/  # 省份级别地图数据
│   └── geometryCouties/   # 城市级别地图数据
└── README.md              # 项目说明文档
```

## 数据来源

地图数据基于开源的中国行政区划GeoJSON数据，经过优化和校正以确保准确性。

## 浏览器兼容性

- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

## 许可证

MIT License

## 贡献

欢迎提交Issue和Pull Request来改进这个项目。

## 更新日志

### v1.0.0
- 初始版本发布
- 支持基本的地图可视化功能
- 添加交互式操作
- 支持数据输入和颜色映射
- 添加缩放和拖拽功能
- 实现智能标签显示/隐藏
- 添加淡灰色地图背景