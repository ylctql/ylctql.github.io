# Personal Academic Homepage

简约、全英文的个人学术主页模板。暖白背景、衬线标题、绿色点缀，支持手机、键盘导航和打印。纯 HTML / CSS，无构建步骤、第三方脚本或外部字体依赖。

## 填写个人信息

在 GitHub 打开 `index.html`，点击铅笔图标编辑，按中文 `TODO 1` 至 `TODO 12` 注释修改，然后提交。也可以在本地用文本编辑器修改。页面展示全英文，中文注释不会出现在网页中。

优先填写以下三项：

1. **真实英文姓名**：网页标题、`h1`、简介和页脚；应与 OpenReview 注册姓名一致。
2. **真实机构**：首页 `Affiliation` 中的院系 / 实验室和学校 / 机构；同时修改 Contact 中的信息。
3. **OpenReview 注册邮箱**：替换页面两处 `[Your OpenReview registration email]`。文字要完整展示，可改为 `<a href="mailto:name@university.edu">name@university.edu</a>`。

其余按需填写：当前身份、简介、研究方向、教育经历与所在城市。所有方括号文字均为占位内容，提交给 OpenReview 前请替换或删除。

论文、Google Scholar、ORCID、GitHub、CV 的代码示例已放在 HTML 注释中，提供真实内容后再启用。没有论文时，可以删除 Publications 整个章节以及顶部和侧栏的对应导航；不要把示例当作真实成果。简历可上传到 `assets/cv.pdf`，并启用对应链接。

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

[OpenReview 官方注册说明](https://docs.openreview.net/getting-started/creating-an-openreview-profile/signing-up-for-openreview) 明确指出，有效个人主页应显示**姓名、所属机构和注册 OpenReview 的邮箱**。本模板为这三项预留了醒目位置，但空白模板本身不满足身份核验需要。

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
```

双击 `index.html` 可直接预览。调整主题色可修改 `assets/style.css` 顶部的 `--paper`、`--ink` 和 `--green`。
