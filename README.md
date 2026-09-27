# SafariGoogleRedirect

当 iPhone 地区设置为中国大陆, Safari 设置为谷歌搜索时, Safari 的区域行为是将请求转发至 Google 中国（`www.google.cn`）并展示 google.com.hk 的重定向页面，该脚本则把搜索请求自动传递至 Google 国际版（`www.google.com`）无需确认, 直接搜索. iPhone 地区现在可放心设置为中国大陆, 不用更改地区。  

---

## 功能特性

- **附加: 优化 URL 构造**  
  构造最简洁搜索 URL，仅保留 `q`（搜索关键词）参数，去除多余参数（如 `hl`、`ie`、`oe`、`client` 等），增强隐私安全, 保证搜索 URL 干净、统一。  

- **附加: 加载动画**  
  在搜索结果呈现前，页面显示 **Google Logo + CSS Loading 动画**。  

- **深浅色主题自适应**  
  自动检测 iOS 系统深色/浅色模式，动画颜色和背景色随主题变化：
  - 浅色模式 → 白色背景 + 蓝色加载动画  
  - 深色模式 → 深灰背景 + 亮蓝加载动画  

- **兼容性**  
 覆盖 iOS 地区设置为中国大陆, Safari 设置为谷歌搜索的所有iOS版本。


---

## 安装方法

1. 在 iPhone 安装 **Tampermonkey** 或 任意 **提供用户脚本功能** 的 Safari 浏览器扩展, 有收费的, 有免费的自行选择, 任意一个都可以.
2. 在你选择使用的扩展中, 添加脚本, URL为 [https://raw.githubusercontent.com/garinasset/SafariGoogleRedirect/main/SafariGoogleRedirect.user.js](https://raw.githubusercontent.com/garinasset/SafariGoogleRedirect/main/SafariGoogleRedirect.user.js) 
3. 下载添加后, 启用 **Safari · Google 重定向**
4. 在 Safari 中选择 Google 作为搜索引擎, 在地址栏键入关键词, 进行搜索时，脚本会自动
   1. 显示加载动画 (Logo + 动画).
   2. 自动跳转到 Google 国际版 [www.google.com](www.google.com) 的搜索结果页面, 搜索页面使用的就是你搜索的关键词哦.

---


## 更新与反馈

- GitHub 仓库：[https://github.com/garinasset/SafariGoogleRedirect](https://github.com/garinasset/SafariGoogleRedirect)  
- Issues & Bug 报告：[https://github.com/garinasset/SafariGoogleRedirect/issues](https://github.com/garinasset/SafariGoogleRedirect/issues)  
- 自动更新：脚本内配置了 `@updateURL` 指向 GitHub Raw 文件，用户脚本扩展 会自动检查更新 (如果你使用的 Safari 用户脚本扩展支持自动更新).

---

## 许可证

MIT License
