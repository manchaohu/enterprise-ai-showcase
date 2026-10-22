# 网站发布与验收

本仓库为 **Public**，与私人技术实验仓库 `enterprise-ai-tech-lab` 完全独立。

发布白名单现为四份 HTML：`index.html`、`demo24/index.html`、`demo25/index.html`、`demo23/index.html`。读者教程可直接提交主分支，公开试阅后再按人工反馈修订，不必每次走 PR/MR。真实实验模型、图片和私人仓库源码不被复制。它们是静态教程；示意 SVG 不是实际模型预测图。

首次配置时在 [Settings → Pages](https://github.com/manchaohu/enterprise-ai-showcase/settings/pages) 的 **Build and deployment → Source** 选择 **GitHub Actions**。部署脚本只上传白名单内的四份 HTML，每次 main 的教程文件更新会自动发布。若首次合并后自动部署尚未成功，可在 [Actions](https://github.com/manchaohu/enterprise-ai-showcase/actions) 手动运行 `Publish AI reader site`。

成功部署后的项目站点地址应为：

https://manchaohu.github.io/enterprise-ai-showcase/

部署通过后须实际验证首页、`demo24/`、`demo25/`、`demo23/` 可访问和章节互相跳转。在 GitHub Actions 显示 SUCCESS 前，网址只能视为预期地址。
