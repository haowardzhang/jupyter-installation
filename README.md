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
