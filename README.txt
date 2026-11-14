CHENXI / TAN ZE — 静态作品集部署版

使用
双击 index.html 可查看本地图片和文字；YouTube 视频需要网络。
网站使用 HTML/CSS，不需要 Node、构建工具或后台。
assets/ 只保留 HTML/CSS 实际使用的展示图片和本地字体。
按用户要求已删除未展示的原图、旧展示图和未引用素材。
display-assets.json 的 source、IMAGE-MAP.csv 的 source_reference 仅为历史来源记录，不代表保留本地原图。

修改
首页、About Me 的文字直接修改 HTML。展板内文字需修改设计素材后重新导出。
替换图片时更新 HTML、IMAGE-MAP.csv 和 display-assets.json。

上传 GitHub
解压 chenxi-portfolio-deploy.zip，将里面的内容上传仓库根目录，不要上传 ZIP 本身。
根目录直接包含 index.html、styles.css、assets/ 和 render.yaml。

Render
New > Static Site，连接 GitHub 仓库。
Root Directory 留空；Build Command 填 echo static；Publish Directory 填 .
不需要 Start Command 或环境变量。

GitHub Pages
Settings > Pages > Deploy from a branch，选择 main 与 /(root)。已附 .nojekyll。

重新打包
在本地项目执行 python3 tools/package_site.py；运行网站不需要 Python。
本次仅本地清理与打包，没有推送 GitHub 或发布到 Render。
