# Abaqus Param Runner


启动方式：

```text
双击 run_latest.bat
```

也可以直接进入具体版本：

```text
双击 versions\v1.4.4\run.bat
```

如果双击后还是打不开：

```text
双击 versions\v1.4.4\run_debug.bat
```

`run_debug.bat` 会把 Python 路径、Python 版本、语法检查结果和报错信息显示出来，窗口不会立刻关闭。


需要：

- Windows
- Python 3，且安装时勾选 Tcl/Tk 或 tcl/tk and IDLE
- Abaqus 命令可用，或者在软件里把 Abaqus 命令改成完整路径

软件会自动寻找 Abaqus 命令，顺序是：

1. 读取上次保存的设置。
2. 查找系统里的 `abaqus` 命令。
3. 查找常见路径，例如 `D:\ABAQUSAPP\abaqus.bat`。

关闭软件或开始运行时，会自动保存当前设置到：

```text
versions\v1.4.4\runner_config.json
```

如果运行日志提示“找不到 Abaqus 命令”，说明 Windows 找不到 `abaqus`。处理方法：

1. 在软件里点击 `选择命令`。
2. 找到 Abaqus 的启动脚本，通常类似：

```text
C:\SIMULIA\Commands\abaqus.bat
C:\SIMULIA\Commands\abq2024.bat
C:\SIMULIA\Commands\abq2023.bat
```

不同版本名称可能不同，选择你电脑里真实存在的 `.bat/.cmd/.exe` 即可。
