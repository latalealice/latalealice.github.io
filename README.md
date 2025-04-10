
# 学术主页

![pages-build-deployment](https://github.com/academicpages/academicpages.github.io/actions/workflows/pages/pages-build-deployment/badge.svg)

Academic Pages 是用于学术网站的 Github Pages 模板


# 开始

1. 如果您没有 GitHub 帐户，请注册一个 GitHub 帐户并确认您的电子邮件（必填）
1. 单击右上角的 “Use this template” 按钮
1. 在“New repository（新建仓库）”页面上，输入您的仓库名称为 “[your GitHub username].github.io”，这也是您网站的 URL
1. 设置站点范围的配置并添加您的内容
1. 将任何文件（如 PDF、.zip 文件等）上传到 files/ 目录。它们将显示在 https://[你的 GitHub 用户名].github.io/files/example.pdf  
1. 通过转到存储库设置中的“GitHub 页面”部分来检查状态
1. （可选）使用 markdown_generator 文件夹中的 Jupyter 笔记本或 python 脚本从 TSV 文件生成用于出版物和演讲的 markdown 文件

有关更多信息 ，请访问 https://academicpages.github.io/


## 本地运行

当您最初使用网站时，能够在将更改推送到GitHub之前在本地预览更改非常有用。要在当地工作，您需要：

1. 克隆存储库并进行更新，如上所述
1. 确保您已安装ruby-dev、bundler和nodejs： sudo apt install ruby-dev ruby-bundler nodejs
1. 运行bundle install以安装ruby依赖项。如果出现错误，请删除Gemfile.lock并重试
1. 运行 jekyll serve -l -H localhost 生成 HTML 并从 localhost：4000 提供它，本地服务器将自动重建并在更改时刷新页面


# 维护  

模板的Bug报告和功能请求应通过[submitted via GitHub](https://github.com/academicpages/academicpages.github.io/issues/new/choose)提交。有关如何设置模板样式的问题，请随时在[new discussion on GitHub](https://github.com/academicpages/academicpages.github.io/discussions)上发起新的讨论

这个仓库是由[Stuart Geiger](https://github.com/staeiou)从[Minimal Mistakes Jekyll Theme](https://mmistakes.github.io/minimal-mistakes/)中分叉出来的，该主题是©2016年的Michael Rose，并在MIT许可证下发布（参见LICENSE.md）。它目前由Robert Zupko维护，欢迎其他维护者

## 错误修复和增强功能

如果您想将错误修复和增强功能作为拉取请求提交，则需要复刻此存储库[fork](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo)，而不是将其用作模板。这也将允许您将模板副本同步到fork[synchronize your copy](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/syncing-a-fork)

像Academic Pages这样的模板主题存在一个后勤问题，这使得修复和更新核心主题变得有点棘手。如果使用此模板并对其进行自定义，则在尝试同步时可能会遇到合并冲突。如果要保存各种 .yml 配置文件和 Markdown 文件，可以删除存储库并再次复刻。或者您可以手动修补
