# How to Publish Version 1.0 Release on GitHub

This guide will help you create a GitHub release for version 1.0.0 of the schedule/timetable management system.

## Prerequisites
- You must be logged into GitHub
- You must have write access to the repository

## Steps to Create Release v1.0.0

### 1. Navigate to Releases Page
1. Go to your repository: https://github.com/CrocodileWoodGordon/schedule
2. Click on "Releases" in the right sidebar (or go to https://github.com/CrocodileWoodGordon/schedule/releases)
3. Click the "Draft a new release" button

### 2. Create Release Tag
- **Tag version**: `v1.0.0`
- **Target**: Select the commit `1b39355` (the commit before version 1.1 changes)
  - Alternatively, you can tag from `v1.0.html` file in the current branch

### 3. Release Title
```
Version 1.0.0 - Initial Release
```

### 4. Release Description
Copy and paste the following markdown:

```markdown
# 课程表管理系统 v1.0.0 - 首次发布 / Timetable Management System v1.0.0 - Initial Release

[English](#english) | [中文](#中文)

---

## 中文

### 🎉 首次发布

这是课程表管理系统的首个正式版本，提供完整的课程表管理功能。

### ✨ 主要功能

#### 📅 课程管理
- **添加课程**：选择星期、起始/结束节次，输入课程信息快速添加
- **删除课程**：支持多选删除，按住 Ctrl 可选择多个时间段
- **课程冲突检测**：添加课程时自动检测时间冲突，提供"覆盖"和"跳过"选项
- **清空功能**：一键清空所有课程数据

#### 🎨 视觉效果
- **自动配色**：每门不同的课程自动分配独特的渐变色（22种配色方案）
- **课程合并显示**：相邻相同课程自动合并为一个视觉块，隐藏分割线
- **暗色主题**：现代化的深色界面设计，护眼舒适
- **响应式布局**：适配不同屏幕尺寸

#### ⏰ 时间管理
- **自定义时间**：点击左侧时间栏可编辑上课时间（支持回车保存、ESC取消）
- **恢复默认**：一键恢复初始时间设置
- **时间持久化**：自定义时间自动保存到浏览器本地存储

#### 💾 数据持久化
- 使用 localStorage 自动保存所有数据
- 刷新页面后数据不丢失

### 📦 使用方法

1. 下载 `v1.0.html` 文件
2. 在浏览器中打开文件即可使用
3. 无需安装，无需服务器

### 🔧 技术栈
- HTML5 + CSS3 + JavaScript (ES6+)
- 纯前端实现，无依赖
- CSS Grid 布局
- localStorage 数据持久化

### 🌐 浏览器兼容性
- Chrome/Edge 90+
- Firefox 88+
- Safari 14+

### ⚠️ 注意事项
- 数据仅存储在浏览器本地
- 清除浏览器缓存会删除所有数据
- 建议定期截图备份重要课程表信息

### 🚀 下一步计划
v1.1.0 版本将包含：
- ✅ 导入/导出课程表功能（JSON/CSV格式）

---

## English

### 🎉 Initial Release

This is the first official release of the Timetable Management System, providing complete course schedule management functionality.

### ✨ Main Features

#### 📅 Course Management
- **Add Courses**: Select day, start/end period, and enter course information to add quickly
- **Delete Courses**: Support multi-selection deletion, hold Ctrl to select multiple time slots
- **Conflict Detection**: Automatically detect time conflicts when adding courses, provide "Overwrite" and "Skip" options
- **Clear All**: Clear all course data with one click

#### 🎨 Visual Effects
- **Auto Color Scheme**: Each different course is automatically assigned a unique gradient color (22 color schemes)
- **Course Merging**: Adjacent identical courses are automatically merged into one visual block, hiding dividers
- **Dark Theme**: Modern dark interface design, eye-friendly and comfortable
- **Responsive Layout**: Adapts to different screen sizes

#### ⏰ Time Management
- **Custom Time**: Click on the left time column to edit class time (support Enter to save, ESC to cancel)
- **Restore Default**: Restore initial time settings with one click
- **Time Persistence**: Custom time automatically saved to browser local storage

#### 💾 Data Persistence
- Automatically save all data using localStorage
- Data is not lost after refreshing the page

### 📦 Usage

1. Download the `v1.0.html` file
2. Open the file in your browser to use
3. No installation required, no server needed

### 🔧 Tech Stack
- HTML5 + CSS3 + JavaScript (ES6+)
- Pure frontend implementation, no dependencies
- CSS Grid layout
- localStorage data persistence

### 🌐 Browser Compatibility
- Chrome/Edge 90+
- Firefox 88+
- Safari 14+

### ⚠️ Notes
- Data is stored locally in browser only
- Clearing browser cache will delete all data
- It is recommended to regularly take screenshots to backup important timetable information

### 🚀 Next Steps
Version 1.1.0 will include:
- ✅ Import/export timetable functionality (JSON/CSV format)

---

### 📥 Download

Download the `v1.0.html` file from the assets below and open it in your browser.

**Checksum (SHA256)**: (Will be calculated by GitHub)

---

**Full Changelog**: https://github.com/CrocodileWoodGordon/schedule/commits/v1.0.0
```

### 5. Upload Release Asset
1. In the "Attach binaries" section at the bottom
2. Drag and drop or click to upload the `v1.0.html` file from your repository
3. This will be the downloadable file for version 1.0.0

### 6. Publish Release
1. Make sure "Set as the latest release" is **unchecked** (since v1.1.0 is the latest)
2. Click "Publish release"

---

## Verify Release

After publishing, verify that:
- The release appears at https://github.com/CrocodileWoodGordon/schedule/releases
- The `v1.0.html` file is downloadable
- The release is tagged as `v1.0.0`

---

## Notes

- Version 1.0.0 represents the original version without import/export features
- The `v1.0.html` file in the repository is an exact copy of the original `index.html` before it was updated to v1.1.0
- Users who want to use the original version can download `v1.0.html` from the release
- Version 1.1.0 (current `index.html`) includes all v1.0.0 features plus import/export functionality
