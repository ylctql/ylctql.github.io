# Personal Academic Homepage

Liangchen Yan 的全英文个人学术主页。暖白背景、衬线标题、绿色点缀，支持手机、键盘导航和打印。纯 HTML / CSS，无构建步骤、第三方脚本或外部字体依赖。

## 填写个人信息

在 GitHub 打开 `index.html`，点击铅笔图标编辑，搜索中文 `UPDATE` 注释并修改对应内容，然后提交。也可以在本地用文本编辑器修改。页面展示全英文，中文注释不会出现在网页中。

优先填写以下三项：

1. **真实英文姓名**：网页标题、`h1`、简介和页脚；应与 OpenReview 注册姓名一致。
2. **真实机构**：首页 `Affiliation` 中的院系 / 实验室和学校 / 机构；同时修改 Contact 中的信息。
3. **OpenReview 注册邮箱**：保持顶部和 Contact 两处邮箱一致。若邮箱变化，需同时修改显示文字和 `mailto:` 链接。

其余按需填写：当前身份、简介、研究方向、教育经历与所在城市。主要维护位置和注意事项见 [UPDATE-NOTES.md](UPDATE-NOTES.md)。

GitHub 和邮箱链接已启用。Publications 章节模板保留在 HTML 注释中，补充真实论文后再启用并添加导航。Google Scholar、ORCID 或 CV 链接可在有对应资料后添加；简历可放在 `assets/cv.pdf`。

## GitHub Pages 发布

个人站点仓库建议命名为 `你的GitHub用户名.github.io`，例如 `ylctql.github.io`。文件应直接位于仓库根目录，不能多套一层 `personal-homepage/`。

在仓库 **Settings → Pages → Build and deployment** 中设置：

- Source：**Deploy from a branch**
- Branch：**main**
- Folder：**/ (root)**
- 点击 **Save**。

等待 Pages 构建完成后，打开 Settings → Pages 显示的 **Visit site** 链接。该账号的个人站点预期为 `https://ylctql.github.io/`，以 GitHub 显示的实际地址和部署状态为准。

后续修改 `index.html` 并提交即可自动更新。`.nojekyll` 用于直接发布静态文件。若使用 GitHub Free，Pages 站点源码仓库需为公开仓库。

## OpenReview Homepage URL

[OpenReview 官方注册说明](https://docs.openreview.net/getting-started/creating-an-openreview-profile/signing-up-for-openreview) 明确指出，有效个人主页应显示**姓名、所属机构和注册 OpenReview 的邮箱**。当前页面已展示姓名、机构及学校邮箱；请确认邮箱与 OpenReview 注册资料一致。

提交前请检查：

- 真实姓名、机构和注册邮箱已填写，首页直接可见。
- 已使用无痕窗口确认网站可公开访问，无须登录。
- Homepage URL 填写发布后网站的完整 HTTPS 地址，不填写编辑页或仓库设置页。
- 网页内容与 OpenReview 个人资料一致，未保留虚构经历或占位成果。
- 机构或院系的通用首页不能代替个人主页。

没有机构时，请如实说明 Independent Researcher，并参考 [OpenReview 独立研究者说明](https://docs.openreview.net/getting-started/frequently-asked-questions/i-am-an-independent-researcher-how-do-i-sign-up)，补充其要求的个人背景及相关资料。

满足主页内容要求有助于审核，但不能保证 OpenReview 账户一定获批。

## 文件

```text
index.html          # 所有网页内容与个人信息，在此填写
assets/style.css    # 排版、配色、手机与打印样式
assets/favicon.svg  # 简洁叶片图标
.nojekyll           # 关闭 Jekyll 处理
README.md           # 本说明
UPDATE-NOTES.md     # 后续维护提示
```

双击 `index.html` 可直接预览。调整主题色可修改 `assets/style.css` 顶部的 `--paper`、`--ink` 和 `--green`。
