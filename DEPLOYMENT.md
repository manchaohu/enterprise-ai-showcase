# 公开教程发布与验收 / Public Tutorial Deployment and Acceptance

[中文](#中文) · [English](#english)

## 中文

网站：[https://manchaohu.github.io/enterprise-ai-showcase/](https://manchaohu.github.io/enterprise-ai-showcase/)；英文入口：[https://manchaohu.github.io/enterprise-ai-showcase/en/](https://manchaohu.github.io/enterprise-ai-showcase/en/)。

**部署隔离：** 此 Public 仓库与私有 `enterprise-ai-tech-lab` 独立。只发布白名单中的 **14 个 HTML**：中文首页、中文 6 篇、英文首页、英文 6 篇；不发布模型、原录音、第三方照片、私有源码或数据。所有实验来源和许可证限制必须如实标记。

**操作流程：** 读者版 HTML 可直接提交 `main`，无需逐篇 PR/MR。文件变动触发 `.github/workflows/pages.yml`，先验证所有页面和站内相对链接，再上传 Pages Artifact，最后由 `actions/deploy-pages@v4` 发布。发布后人工分别检查中英文首页、六篇中文、六篇英文及每页语言切换链接。

**首次设置：** 仓库 [Settings → Pages](https://github.com/manchaohu/enterprise-ai-showcase/settings/pages) 中，将 Build and deployment / Source 选为 GitHub Actions。现已存在成功部署记录；若工作流失败，不能把页面更新称为上线成功。可从 [Actions](https://github.com/manchaohu/enterprise-ai-showcase/actions) 查看准确运行和部署状态。

**质量约束：** 同一技术事实、运行 ID、真实数据数字、能力边界在中英文保持一致。示意图与实测图分别标明，英文页不能只是空白语言开关；页面不提供实时模型服务。私有仓库的链接可能无法被未经授权的读者打开。人工审读后的修改继续直接提交主分支。

## English

Website: [https://manchaohu.github.io/enterprise-ai-showcase/](https://manchaohu.github.io/enterprise-ai-showcase/). English entry: [https://manchaohu.github.io/enterprise-ai-showcase/en/](https://manchaohu.github.io/enterprise-ai-showcase/en/).

**Isolation:** the public showcase is independent of the private `enterprise-ai-tech-lab` repository. The Pages build publishes exactly **14 whitelisted HTML pages**: one Chinese index, six Chinese lessons, one English index, and six English lessons. Model weights, original audio, third-party photographs, private engineering code, and datasets are not uploaded. All evidence and licensing caveats remain explicit.

**Process:** update reader HTML directly on `main`; a per-page pull request is not required. `.github/workflows/pages.yml` validates file presence and local relative links before packaging a Pages artifact and deploying it with `actions/deploy-pages@v4`. After the deployment succeeds, manually review both catalogs and all twelve lessons, including the Chinese ↔ English navigation on every page.

**Initial settings:** under [Settings → Pages](https://github.com/manchaohu/enterprise-ai-showcase/settings/pages), Build and deployment / Source should be GitHub Actions. Consult actual [Actions results](https://github.com/manchaohu/enterprise-ai-showcase/actions) before claiming any new version is live.

**Editorial acceptance:** both language versions must agree about dates, numeric observations, model identities, evidence run IDs, limitations and demonstrated scope. Distinguish conceptual SVGs from real experimental output. This static website does not host model inference, and private laboratory links may be inaccessible to unauthorized visitors. Correct translated text directly on `main` after reader feedback.
