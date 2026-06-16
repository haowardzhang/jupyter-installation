# jupyter-installation
jupyter-installation


1. 虚拟环境中安装 ipykernel
请确保你的终端提示符最前面带有 (aitest)。如果在，直接运行以下命令：

Bash
uv pip install ipykernel

2. 重新运行注册命令
安装成功后，再次执行你刚才那条命令：

Bash
python -m ipykernel install --user --name=aitest --display-name "aitest"


1. 安装库
在终端（或 Notebook 单元格里）安装 nbimporter：

Bash
uv pip install nbimporter  # 或者 !pip install nbimporter


2. 在代码中使用
在你当前写代码的 Notebook 顶部，先 import nbimporter，然后你就可以像对普通 Python 文件一样，直接 import 另一个 ipynb 文件了！

假设你有一个叫 utils.ipynb 的文件，里面定义了一个 greet() 函数。在同一个文件夹下的另一个 Notebook 里，你可以这样写：

Python
import nbimporter
from utils import greet  # 没错，现在可以直接 import 了！

