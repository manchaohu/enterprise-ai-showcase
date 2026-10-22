# 网站发布与验收

本仓库为 **Public**，与私人技术实验仓库 `enterprise-ai-tech-lab` 完全独立。

发布白名单现为七份 HTML：首页加上 Demo 24、25、23、21、13、27 六篇教程。读者教程可直接提交主分支，公开试阅后再按人工反馈修订，不必每次走 PR/MR。真实实验模型、图片和私人仓库源码不被复制。它们是静态教程；示意 SVG 不是实际模型预测图。

首次配置时在 [Settings → Pages](https://github.com/manchaohu/enterprise-ai-showcase/settings/pages) 的 **Build and deployment → Source** 选择 **GitHub Actions**。部署脚本只上传白名单内的七份 HTML，每次 main 的教程文件更新会自动发布。若首次合并后自动部署尚未成功，可在 [Actions](https://github.com/manchaohu/enterprise-ai-showcase/actions) 手动运行 `Publish AI reader site`。

成功部署后的项目站点地址应为：

https://manchaohu.github.io/enterprise-ai-showcase/

部署通过后须实际验证首页、`demo24/`、`demo25/`、`demo23/`、`demo21/`、`demo13/`、`demo27/` 可访问和章节互相跳转。在 GitHub Actions 显示 SUCCESS 前，网址只能视为预期地址。

## 批量教程扩展（2026-10-22）

在前三篇人工效果获得认可后，第一轮再直接发布三篇不同机制的读者教程：Demo 21 时序预测、Demo 13 真 RAG、Demo 27 SQLite 关系图多跳。新的真实可视化：Demo 21 由已有核验报告中的六个 MAE 数值重新绘制比较图；Demo 27 图依据源文件 `data/evidence.json` 的五条显式边绘制；Demo 13 图为严格标记的代码机制示意。三篇都不把示意图误称真实模型输出。

今后批量发布仍以可追溯证据、用户人工读后修改为准。批量扩充只增加公开教程数量，不增加已有 27 项 Demo 数量。无需 PR，但须等待 GitHub Pages 自动构建/部署成功并检查站内链接。
