# vscode 模板项目

本项目中需要涉及的内容包括：

- workspace 配置文件
- setting 配置文件
- 源代码目录
- 单元测试目录
- .gitignore文件
- python.code-snippets
- 终端配置

本项目不含python虚拟目录的安装配置，可参考本文最后部分操作。

本项目的部分配置是针对vscode插件的配置，本文最后部分有推荐的vscode插件安装清单



## 项目使用方法

下载本项目中 \\python项目\\python_prj.zip 文件，加压缩到本地，即可得到默认项目目录



## 项目目录说明

项目目录按以下方式安排：

**\-\- .vscode**      vscode项目配置文件

​	*\-\- python.code-snippets*     python代码片段配置文件

​	*\-\- settings.json*                     项目配置文件

**\-\- doc**             文档目录

**\-\- src**               源代码目录

**\-\- src_test**       单元测试源代码目录

*\-\- .gitignore*            GIT忽略清单

*\-\- README.md*       项目说明



## 配置说明



### workspace 配置文件

配置文件都存放在项目目录中，即.vscode中的setting.json目录中。

在本处，保持最简单的配置：

```json
{
	"folders": [
		{
			"path": "."
		}
	],
	"settings": {		
	}
}
```

### setting 配置文件

是项目级别的配置文件，在.vscode目录下

settings中有以下内容的默认配置：

- python解析器，python.pythonPath
- python语法检查，python.linting.xxx
- python单元测试，python.testing.xxx
- 插件配置：
  - todo-tree系列
  - 

### .gitignore文件

为上传github库时候要忽略的文件配置清单，项目中可按此项目配置，不用调整。



### python.code-snippets

python代码片段，可使用以下的代码片段：

- HEADER
- DEF（建议删除）

除去用户级别外，安装phthon插件后有基础的代码片段，所以不建议改这部分



## python虚拟环境的配置

推荐使用Anaconda软件，然后按以下步骤操作：

1. **创建虚拟环境**

   在命令行中输入：

```dos
python -m venv 虚拟环境名 --system-site-packages
```

执行后，在当前目录下生成新的以 虚拟环境名 为名称的目录；

--system-site-packages参数的意思是继承环境的所有Lib。

2. **配置.pth文件**

打开 

3. **vscode中指定虚拟环境**



4. 安装第三方库

   

虚拟环境的建立

虚拟环境中安装 第三方库

src和src_test的配置



## vscode插件的安装

**必须的插件清单:**

- Python（Microsoft）
- vscode-icons
- Python Test Explorer for vscode
- Test Explorer UI
- Slack Theme

***推荐的插件清单:***

- atuoDocstring

- Markdown All in one

- TODO Highlight

- Todo Tree

  

下载的离线安装包：

| 插件                            | 离线安装包                                           |
| ------------------------------- | ---------------------------------------------------- |
| Python                          |                                                      |
| vscode-icons                    | vscode-icons-team.vscode-icons-9.6.0.vsix            |
| Python Test Explorer for vscode | LittleFoxTeam.vscode-python-test-adapter-0.3.15.vsix |
| Test Explorer UI                | hbenl.vscode-test-explorer-2.15.0.vsix               |
| Slack Theme                     |                                                      |
|                                 |                                                      |
| atuoDocstring                   |                                                      |
| Markdown All in one             |                                                      |
| TODO Highlight                  |                                                      |
| Todo Tree                       |                                                      |

