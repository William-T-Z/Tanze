CHENXI LIU — 本地静态作品集

开始使用
解压整个文件夹，双击 index.html 即可。不要只拷贝一个 HTML 文件。
不需要 Node、npm、数据库、Wix 账号或付费编辑器。

文件
index.html：首页四个项目的封面、标题、分类和简介。
aboutme.html：个人介绍与肖像。
unspoken-colony.html / silenttower.html / tampered-spring.html / consciousindustry.html：四个项目页。
styles.css：公共字体和排版，末尾为手机适配。
assets/：原尺寸图片与本地字体。图片改成了可辨认的项目名称。
IMAGE-MAP.csv：四个项目的图片顺序及原文件名。
AGENTS.md：学生用 Codex 修改这个文件夹时应遵循的规则。

改文字
用 VS Code 打开整个文件夹。在相应 HTML 搜索原句并修改。
首页标题、项目分类、简介和 About Me 是真实 HTML 文本。
项目详情是原网站的整张作品集展板：图内文字不能在 HTML 里直接修改。
需要从 Figma、PS 或其他原设计文件修改后导出图片，再替换相应展板。

改图片
assets/unspoken-colony-cover.jpg 是对应首页封面（以实际扩展名为准）。
项目详情以“项目名称-01.png、-02.jpg”等依次排列，以 HTML 的 src 和 IMAGE-MAP.csv 为准。
可以直接用同名同格式新图覆盖；换文件名时，同时改 HTML 的 src。
保持原图片比例可减少排版变化。文件名建议使用英文小写字母和短横线。

交给 Codex
让学生把整个文件夹作为项目打开，先读 AGENTS.md。
示例：“把首页 Silent Tower 的简介替换成以下文字……，保留现有排版，检查手机端。”
示例：“把 assets 中我新放的图片替换为 Tampered Spring 第三张展板，其他不变。”
示例：“新增一个作品，沿用首页项目模块和详情页展板结构。材料如下……。”
老师如需提意见，可以把修改清单发给学生，或在其 GitHub 仓库开 Issue，由学生用 Codex 执行。
这不是共同编辑后台，不需要老师持续维护服务器。

上传 GitHub
推荐 GitHub Desktop：新建学生自己的仓库，把本文件夹内容放进仓库根目录，提交后 Publish repository。
根目录应直接包含 index.html、styles.css、assets/ 等，不要多套一层文件夹。
本交付没有替学生建仓库、推送或发布。

部署 Render（纯静态站）
在 Render 选择 New > Static Site，连接学生自己的 GitHub 仓库，选择 main 分支。
Root Directory 留空；Build Command 填 echo static；Publish Directory 填 .
不填 Start Command，不选择 Node Web Service，不需要环境变量。
之后每次向部署分支推送修改，Render 会重新部署。
仓库内 render.yaml 可供使用 Blueprint 时参考。
Render 的流量、构建额度和自定义域名按当时平台套餐规则执行；无需继续支付 Wix 建站订阅。
官方说明：https://render.com/docs/static-sites

也可直接用 GitHub Pages
仓库 Settings > Pages > Deploy from a branch，选择 main 和 /(root)。
已附 .nojekyll。静态文件使用相对路径，也适合仓库子路径部署。
官方说明：https://docs.github.com/en/pages/quickstart

迁移边界
来源：https://lcx525387.wixstudio.com/chenxi-portfolio
抓取日期：2026-11-10。
已迁移公开首页、About Me、四个项目详情，共 28 张原尺寸图片及本地字体。
这是基于公开页面内容的静态重建，不是 Wix 编辑器源工程导出。
保留白底、黑字、粗体导航、大幅封面、双栏项目说明、按顺序展示项目展板的设计。
手机端增加单栏适配。未迁移 Wix 编辑器、广告、统计或云端服务。
Four YouTube players and original image links have now been restored. Videos require internet access and are not downloaded. Local images and text remain available offline.
字体保留原站文件，仅用于本网站延续展示；若另作分发或改作其他项目，请自行核对字体授权。

FIDELITY UPDATE
The six desktop pages were compared in Chrome at 1440px width. Image crops, font sizes, spacing and About Me colors have been restored. The 30px Wix advertisement is omitted.
Pages now display *-display images; originals without this suffix are retained for editing. Update both when replacing artwork. display-assets.json records each display crop.
YouTube requires internet access. With file://, use the YouTube link if embedding is blocked. Playback of all four videos has not been verified.
The readable single-column mobile adaptation is retained. Final mobile verification was interrupted by browser timeouts.
