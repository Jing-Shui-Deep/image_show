# Image URL Viewer - 图片链接提取工具

一个简洁高效的图片 URL 提取和可视化展示工具，帮助你快速从文本中提取图片链接并按行分组展示。

## 功能特点

### 核心功能
- **智能提取**：自动从任意文本中提取图片 URL
- **按行分组**：同一行的多个图片会分组展示，方便对比
- **Key-Value 识别**：自动识别 URL 前的标识符（如 `sourceUrl:`, `targetUrl:` 等）
- **实时统计**：输入时实时统计检测到的图片 URL 数量

### 展示功能
- **灵活布局**：可自定义一行展示几组、每组几列图片
- **图片预览**：点击图片可查看大图
- **URL 列表**：提供完整的 URL 列表视图，支持一键复制
- **数据详情**：每组图片可展开查看原始文本和 URL 详情

### 交互功能
- **快捷复制**：每个 URL 都提供快速复制按钮
- **批量复制**：支持一键复制所有 URL
- **可折叠面板**：布局设置和 URL 列表可按需显示/隐藏
- **响应式设计**：完美适配桌面端和移动端

## 支持的 URL 格式

- 标准 HTTPS/HTTP URL：`https://example.com/image.jpg`
- 协议相对 URL：`//cdn.example.com/photo.png`
- Markdown 图片格式：`![alt](https://example.com/image.gif)`
- 带查询参数的 URL：`https://example.com/image.png?size=large`

## 支持的图片格式

jpg, jpeg, png, gif, webp, svg, bmp, ico

## 使用方法

### 基本使用

1. **输入文本**
   - 在输入框中粘贴包含图片 URL 的文本
   - 支持多行输入，每行可包含一个或多个 URL

2. **提取并展示**
   - 点击"🚀 提取并展示"按钮（或使用快捷键 `Ctrl/Cmd + Enter`）
   - 图片将按行分组展示

3. **查看大图**
   - 点击任意图片可查看大图
   - 按 `ESC` 键关闭预览

### 高级功能

#### 布局设置
1. 点击"⚙️ 布局设置"按钮显示设置面板
2. 调整参数：
   - **一行展示组数**：控制横向显示几组图片（1-6）
   - **每组图片列数**：控制每组内图片的列数（1-6）
3. 点击"✓ 应用布局"生效

#### URL 列表
1. 点击"📋 URL列表"按钮显示列表面板
2. 查看所有提取的 URL 及其对应关系
3. 点击"📋 复制全部"一键复制所有 URL

#### 数据详情
- 每组图片下方都有"📋 数据详情"面板
- 点击可展开查看：
  - 原始文本内容
  - 提取的所有 URL 及其 Key 标识

## Key-Value 识别示例

当 URL 前有标识符时，工具会自动识别并在展示时标注：

```
sourceUrl: https://example.com/before.jpg
targetUrl: https://example.com/after.jpg
```

展示时会显示：
- 图片 1 - **sourceUrl**
- 图片 2 - **targetUrl**

## 快捷键

- `Ctrl/Cmd + Enter`：提取并展示图片

## 技术特点

- **零依赖**：纯 HTML + CSS + JavaScript，无需任何外部依赖
- **单文件**：所有代码集成在一个 HTML 文件中
- **即开即用**：直接用浏览器打开即可使用
- **离线可用**：无需网络连接

## 使用场景

- **UI 设计对比**：对比设计稿的前后版本
- **图片资源管理**：整理和预览图片资源链接
- **内容审核**：批量查看和对比图片内容
- **开发调试**：快速预览 API 返回的图片 URL
- **文档整理**：从文档中提取图片链接并可视化

## 浏览器兼容性

支持所有现代浏览器：
- Chrome/Edge（推荐）
- Firefox
- Safari
- Opera

## 本地运行

1. 克隆或下载本项目
2. 用浏览器打开 `index.html` 文件
3. 开始使用

## 示例输入

```
比对图片 1:
sourceUrl: https://picsum.photos/400/300?random=1
targetUrl: https://picsum.photos/400/300?random=2

比对图片 2:
sourceUrl: https://picsum.photos/400/300?random=3
targetUrl: https://picsum.photos/400/300?random=4
```

## 更新日志

### v1.0.0
- 初始版本发布
- 支持基本的 URL 提取和展示功能
- 支持自定义布局
- 支持 Key-Value 识别
- 响应式设计

## License

MIT License

## 作者

guotao

---

如有问题或建议，欢迎提出 Issue！
