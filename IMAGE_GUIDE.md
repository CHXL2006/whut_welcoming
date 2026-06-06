# 图片引用指南

## 快速开始

### 文件夹结构
```
images/
├── dorm/          # 宿舍相关图片
├── food/          # 食堂相关图片
├── campus/        # 校园设施图片
└── club/          # 社团组织图片
```

## 使用方法

### 方法一：相对路径（本地开发）
```html
<img src="./images/dorm/yu14.jpg" alt="余14舍宿舍">
<img src="./images/food/canteen1.jpg" alt="食堂">
```

### 方法二：GitHub 原始 URL（生产环境推荐）
```html
<img src="https://raw.githubusercontent.com/CHXL2006/whut_welcoming/main/images/dorm/yu14.jpg" alt="余14舍宿舍">
```

### 方法三：jsDelivr CDN（加速）
```html
<img src="https://cdn.jsdelivr.net/gh/CHXL2006/whut_welcoming@main/images/dorm/yu14.jpg" alt="余14舍宿舍">
```

## 上传图片步骤

1. 在 GitHub 仓库中打开相应文件夹（如 `images/dorm/`）
2. 点击 "Add file" → "Upload files"
3. 选择要上传的图片文件
4. 在 Commit message 中写入描述
5. 提交更改

## 替换 HTML 中的外部 URL

当前 HTML 使用外部 URL：
```html
<img src="https://modao.cc/agent-py/media/user_assets/..." alt="...">
```

应改为：
```html
<img src="https://raw.githubusercontent.com/CHXL2006/whut_welcoming/main/images/[folder]/[filename]" alt="...">
```

## 好处

✅ 版本控制 - 图片被纳入 Git 版本管理  
✅ 加载速度 - 使用 CDN 加速  
✅ 可靠性 - 无需依赖第三方服务  
✅ 隐私保护 - 所有资源都在自己的仓库中
