# 本项目的修改规则

## 目标与技术
这是从学生原 Wix 作品集迁移的独立静态站。保持双击 index.html 可用。
只用 HTML/CSS；当前没有 JavaScript 交互、构建工具、依赖或后台。
除非学生明确需要新功能，不引入 React、Node、数据库、CMS、账号或图片上传后台。
所有图片和字体必须位于 assets/，所有站内链接使用相对路径。

## 视觉规则
- 白底黑字，图片承担项目视觉，避免另加渐变、卡片阴影和圆角装饰。
- 公共导航：左侧 CHENXI LIU，右侧 PROJECTS 与 ABOUT ME；使用粗体无衬线字体。
- 桌面左右留白约 4%，首页大图后跟两栏说明：左标题，右分类与简介。
- 桌面标题约 20px、正文 16px；不要把图内的排版当成网页字体调整。
- 700px 以下：首页说明变为单栏，导航仍可访问，正文不应横向溢出。
- 四个项目保持自己的图片风格与原有顺序。详情页图片完整显示，禁止裁去展板文字。
- 保留 About Me 的代码式介绍表达；只修改用户要求的实际内容。

## 内容与素材
首页和 About Me 的文字直接在 HTML 修改。
详情页展板内的文字属于位图，需要用户提供修改后的素材；不要声称修改 HTML 即可更改它。
不编造项目资料、研究、数据、采访、成果和经历。
图片文件使用描述性英文名，并同步更新 IMAGE-MAP.csv 和 HTML 引用。
新增作品时沿用 article.project 和 .panels 结构。保留图片 alt 文本。

## 验证与发布
检查受影响页面桌面和手机布局、站内链接、图片、字体和双击打开效果。
保持没有外部运行时资源依赖；本网站无需网络便能显示内容。
用户仅要求本地修改时不要自动推送或发布。
本文件是仓库级规则，不是安装到 Codex 全局的 skill。

## Fidelity update (takes precedence over earlier offline wording)
YouTube iframes and external video links are intentional and require internet. Only images, fonts and text are offline. Do not claim video files were downloaded.
Desktop CSS uses vw dimensions measured at 1440px. Preserve these unless redesign is requested. Omit the original 30px Wix advertisement.
Display images use the -display suffix; originals are retained. Update display and original references when replacing an image. Preserve video slots and image links.
