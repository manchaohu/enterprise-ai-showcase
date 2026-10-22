# 公开教程发布与验收 / Public Tutorial Deployment and Acceptance

[中文](#中文) · [English](#english)

## 中文

网站：[中文首页](https://manchaohu.github.io/enterprise-ai-showcase/) · [English](https://manchaohu.github.io/enterprise-ai-showcase/en/)。

**当前范围：27 项 Demo 的中英双语公开阅读入口。** 其中 6 项是原有完整图文教程，21 项是首版技术导读。每项至少包括一个中文页面 `demoXX/index.html` 与一个英文页面 `en/demoXX/index.html`。两份目录加 54 份内容，总共 **56 页**。这不意味着 21 份新增导读已达到深度图文教程的成熟度。

**发布隔离：** GitHub Pages 的 `.github/workflows/pages.yml` 从 Public 仓库直接构建，**只复制白名单 56 份静态 HTML**，不发布私有 `enterprise-ai-tech-lab` 源码、模型权重、原录音、第三方照片或原始训练数据。源码与原始 Actions 链接保留供已授权读者溯源。

**操作流程：** 可以直接提交 `main`，无需每篇 PR。更新 `index.html`、`demo*/**`、`en/**` 或 Pages 工作流将触发构建。CI 检查 56 文件齐全、相对链接能定位到已发布页面、每项语言切换存在、首页各有 27 张技术卡，再上传 Artifact 和执行 GitHub Pages 部署。**只有对应 Actions build 与 deploy 均成功，才能声称本次新增内容已部署。**

**质量要求：** 中英版本的事实、样本数量、模型名称、关键数字、许可和边界保持一致。示意流程必须与真实输出区分；不能把程序模拟调用写成模型自主行为，也不能把限制范围成功写成真实业务准确率。6 篇完整教程与 21 篇待深化导读应持续分开展示。后续优先为导读补现实场景、真正可展示的授权素材与实验结果图。读者反馈可直接在主分支修订。

## English

Live site: [Chinese catalog](https://manchaohu.github.io/enterprise-ai-showcase/) · [English catalog](https://manchaohu.github.io/enterprise-ai-showcase/en/).

**Scope: 27 public bilingual Demo entries.** Six are established full illustrated tutorials and 21 are initial technical guides, not yet equivalent in editorial depth. Each Demo has `demoXX/index.html` and `en/demoXX/index.html`, giving **56 static HTML pages** including both catalogs.

**Isolation:** the GitHub Pages workflow stages an exact whitelist of 56 HTML files from this Public repository. The private `enterprise-ai-tech-lab` source, model weights, restricted media and raw training datasets are not published. Source and Actions links may require authorization.

**Process:** commit to `main` with no per-page PR/MR. Changes to `index.html`, `demo*/**`, `en/**` or the workflow trigger deployment. CI validates every page, internal relative links, bilingual counterpart navigation and exactly 27 cards in each catalog before upload and Pages deployment. A successful build and deploy in [Actions](https://github.com/manchaohu/enterprise-ai-showcase/actions) is required before treating a new version as published.

**Editorial rules:** English and Chinese must agree on sample counts, model identity, measurements, provenance, license constraints and bounded conclusions. Do not confuse schematic flows with model output, simulated behavior with pretrained inference or demo-level execution with field accuracy. Deepen the 21 initial guides through real evidence-rich visuals, practical scenarios and feedback while keeping the six full tutorials distinct.
