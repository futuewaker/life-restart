# 🌸 人生重启系统 2.0 · Vercel 部署指南

---

## 📁 文件结构（保持这个目录结构上传）

```
life-restart-pwa/
├── index.html               ← 主程序
├── manifest.json            ← PWA 配置
├── sw.js                    ← 离线缓存
├── vercel.json              ← Vercel 配置（必须有）
└── icons/
    ├── icon-192.png
    ├── icon-512.png
    ├── apple-touch-icon.png
    └── favicon-32.png
```

---

## 🚀 部署步骤（全程约 5 分钟）

### 第一步：注册 Vercel
1. 打开 [vercel.com](https://vercel.com)
2. 点击右上角 **「Sign Up」**
3. 选择 **「Continue with GitHub」** 或直接用邮箱注册

### 第二步：部署项目
1. 登录后点击 **「Add New…」→「Project」**
2. 页面左侧选 **「Import Third-Party Git Repository」**，或者直接找到页面底部的 **「Deploy without Git」**（更简单）
3. 如果看到 **「Or deploy from your local files」**，直接把整个 `life-restart-pwa` **文件夹**拖进去
4. 项目名填 `life-restart`（或任意名称）
5. 其他设置一律不动，点击 **「Deploy」**
6. 等待约 30 秒，完成后 Vercel 给你一个网址，例如：
   `https://life-restart.vercel.app`

> 💡 如果没有「拖拽上传」选项，则用 GitHub 方式：
> 1. 在 GitHub 新建仓库，上传这些文件
> 2. 回到 Vercel，点「Import Git Repository」，选刚才的仓库
> 3. 直接 Deploy 即可

---

## 📱 iPhone 安装为 App（关键步骤）

> ⚠️ **必须用 Safari**，Chrome / 微信内置浏览器不支持 iOS 安装 PWA

1. 用 iPhone 的 **Safari** 打开 Vercel 给你的网址
2. 等页面完全加载后，点击底部工具栏中间的 **分享按钮**（方块+向上箭头图标）
3. 在弹出菜单中向下滑，找到 **「添加到主屏幕」**，点击
4. 名称显示「人生重启系统」，直接点右上角 **「添加」**
5. 🎉 退出 Safari，桌面上出现🌸图标

---

## ✅ 安装后的效果

| 功能 | 状态 |
|------|------|
| 全屏显示（无地址栏） | ✅ |
| 离线可用（断网也能打开） | ✅ |
| 数据本地保存 | ✅ |
| 主屏幕图标 | ✅ |
| 刘海/动态岛适配 | ✅ |
| 自动更新（重新部署后） | ✅ |

---

## 💾 数据说明

- 所有数据保存在 **iPhone 本地**（Safari 的 localStorage）
- 不会上传到任何服务器，完全私密
- 点 App 内右上角「💾 保存」按钮可确认写入
- **避免**在 iPhone 设置里「清除 Safari 历史记录和网站数据」，会导致数据丢失

---

## 🔄 以后更新内容

1. 下载新版 `index.html`（从 Claude 获取）
2. 替换 Vercel 项目里的文件（重新上传 / Git push）
3. 手机上打开 App → 下拉刷新 → 自动获取最新版本

---

*🌸 人生重启系统 2.0 · 每一天都比昨天多一点点活力*
