another offline render.


conda env create --file environment.yml

conda install --file requirements.txt -y

pip install -e .

pytest --cov-report=html --cov=relaxrender --ignore=tests/test_relaxrender.py tests


上述指令需要安装anaconda并且在对应的文件夹中打开powershell窗口，输入上述指令，其目的是测试该代码的覆盖率
本代码没有使用给定的组件。
注明：

若遇到找不到模块，或许可以采用如下运行方法，详细请看Python包管理相关知识

**Windows 运行方法之一：**

打开 cmd , cd 到项目根目录，之后设置 临时环境变量 PYTHONPATH 为当前目录，之后在根目录运行你的文件


示例：

```
# cmd
D:   # 磁盘号
cd <项目根目录>
set PYTHONPATH=<relaxrender绝对目录>
python <文件路径>
```

**Linux 运行文件方法之一：**

```
cd <项目根目录>
export PYTHONPATH=<relaxrender绝对目录>
python3 <文件路径>
```


