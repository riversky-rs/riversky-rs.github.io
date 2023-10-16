这是一个用于学术网站的 Github Pages 模板。该模板是由 [Stuart Geiger](https://github.com/staeiou) 从 [Minimal Mistakes Jekyll Theme](https://mmistakes.github.io/minimal-mistakes/) 中 fork 并进行修改的，该主题是 © 2016 Michael Rose 制作的，并在 MIT 许可证下发布。请参见 LICENSE.md。

我认为我已经使其运行得很顺畅并修复了一些重要的 bug，但如果您想改进通用模板/主题，请随时提交问题或拉取请求。

### 注意: 如果您正在使用此存储库并现在收到有关安全漏洞的通知，请删除 Gemfile.lock 文件。

# 说明

1. 如果您还没有 GitHub 帐户，请注册一个并确认您的电子邮件（必需的！）
1. 点击右上方的“fork”按钮，fork [此存储库](https://github.com/academicpages/academicpages.github.io)。
1. 转到存储库的设置（以“Code”开头的选项卡中最右边的项目，应在“Unwatch”下面）。将存储库重命名为“[您的 GitHub 用户名].github.io”，这也将是您的网站 URL。
1. 设置网站范围的配置并创建内容和元数据（见下文 -- 也可以参见[这组diff](http://archive.is/3TPas)，显示为一个名为“getorg-testacct”的用户设置了[示例网站](https://getorg-testacct.github.io)所更改的文件）
1. 将任何文件（例如 PDF、.zip 文件等）上传到 files/ 目录。它们将显示在 https://[您的 GitHub 用户名].github.io/files/example.pdf。
1. 通过转到存储库设置中的“GitHub Pages”部分检查状态
1. （可选）使用 markdown_generator 文件夹中的 Jupyter 笔记本电脑或 python 脚本从 TSV 文件生成出版物和演讲的 markdown 文件。

更多信息请参见 https://academicpages.github.io/

## 在本地运行（不在 GitHub Pages 上，在自己的计算机上提供服务）

1. 克隆存储库并根据上面的说明进行更新
1. 确保已安装 ruby-dev、bundler 和 nodejs：`sudo apt install ruby-dev ruby-bundler nodejs`
1. 运行 `bundle clean` 来清理目录（无需运行 `--force`）
1. 运行 `bundle install` 来安装 ruby 依赖项。如果出现错误，请删除 Gemfile.lock 并重试。
1. 运行 `bundle exec jekyll liveserve` 以生成 HTML 并从 `localhost:4000` 服务。本地服务器将在更改时自动重新构建和刷新页面。

# 更新日志 -- bug 修复和增强功能

使用 ready-to-fork 模板主题的一个物流问题是，很难获得核心主题的 bug 修复和更新。如果您 fork 了此存储库、进行了自定义，然后再次拉取，您可能会遇到合并冲突。如果您想保存各种 .yml 配置文件和 markdown 文件，可以删除存储库并再次进行 fork。或者您也可以手动修补。

为了支持此操作，所有对基础代码的更改都会出现为带有“代码更改”标签的已关闭问题 -- 获取列表 [here](https://github.com/academicpages/academicpages.github.io/issues?q=is%3Aclosed%20is%3Aissue%20label%3A%22code%20change%22%20)。每个问题线程都包括一个评论，链接到单个提交或跨多个提交的差异，因此那些 forked 存储库的人可以轻松地确定他们需要修补什么。