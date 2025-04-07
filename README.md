![Banner 图片](https://user-images.githubusercontent.com/10284570/173569848-c624317f-42b1-45a6-ab09-f0ea3c247648.png)

# n8n 文档库

本仓库用于托管 [n8n](https://n8n.io/) 的文档。n8n 是一款可扩展的工作流自动化工具，帮助您链接任何事物。请在 [docs.n8n.io](https://docs.n8n.io/) 在线浏览文档。


## 在本地预览并构建文档

### 先决条件

* Python 3.8 及以上
* Pip
* n8n 推荐在 Python 开发中使用虚拟环境，例如 [venv](https://docs.python.org/3/tutorial/venv.html)
* Follow the [recommended configuration and auto-complete](https://squidfunk.github.io/mkdocs-material/creating-your-site/#minimal-configuration) guidance for the theme. This will help when working with the `mkdocs.yml` file.
* 本仓库内包含有一个 `.editorconfig` 文件。请确保您的本地编辑器设置**不会覆盖**这些设置。特别是：
	- 不要让您的编辑器将制表符（Tab）替换为空格。这会影响我们的代码示例（因为构建节点时必须保留制表符）。
	- 一个制表符必须等同于四个空格。

### 详细步骤

#### 对于 n8n GitHub 组织内成员：

1. Set up an SSH token and add it to your GitHub account. Refer to [GitHub | About SSH](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/about-ssh) for guidance.
2. Then run these commands:

	```bash
	git clone --recurse-submodules git@github.com:n8n-io/n8n-docs.git
	cd n8n-docs
 	# Set up virtual environment if using one (steps depend on your system)
 	# Install dependencies
	pip install -r requirements.txt
	pip install _submodules/insiders
	```

#### 对于外部贡献者：

Rely on the preview builds on pull requests, or use the free version of Material for MkDocs (most things are the same, some formatting may be missing)

Fork 本仓库，然后：

```
git clone https://github.com/<your-username>/n8n-docs.git
cd n8n-docs
pip install -r requirements.txt
pip install mkdocs-material
```

#### 启动本地预览服务器：

```
mkdocs serve
```

## 如何参与贡献

请阅读这份[贡献](CONTRIBUTING.md)指南。

您还可以在 wiki 中了解[风格指南](https://github.com/n8n-io/n8n-docs/wiki/Styles)。


## 获取支持

如果您有任何问题或困难，请前往 n8n 的论坛发起求助：https://community.n8n.io


## 许可说明

n8n 文档库基于 [**Sustainable Use License**](https://github.com/n8n-io/n8n/blob/master/LICENSE.md) 下的 [fair-code](https://faircode.io/) 许可.

更多关于许可证的信息可以在[许可证文档](https://docs.n8n.io/reference/license/)内查阅。

