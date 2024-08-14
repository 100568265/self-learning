# 把linux gcc配置成环境变量



在Linux系统中，你可以通过修改用户的`.bashrc`或`.bash_profile`文件来配置环境变量。

1. 打开终端。
2. 输入以下命令以编辑`.bashrc`文件：

```bash
nano ~/.bashrc
```

或者如果你使用的是`bash`以外的shell，比如`zsh`，你可能需要编辑`~/.zshrc`。

1. 在文件的末尾添加以下内容，假设GCC安装在`/usr/local/bin`目录下：

```bash
export PATH="/usr/local/bin:$PATH"
```

1. 保存并关闭文件。
2. 使更改生效，运行：

```bash
source ~/.bashrc
```

或者重新开启一个终端窗口。

