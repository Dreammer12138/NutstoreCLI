<h1>Nutstore CLI</h1>

[![PYVERSION](https://img.shields.io/badge/Python-3.7.3-blue)](https://www.python.org)
[![CURL](https://img.shields.io/badge/cURL-green)](http://curl.haxx.se)

Linux环境下的命令行工具

Please click [here](/) to English README.

# 安装

<h2>安装 python3.7 或者更高版本</h2>

以Debian为例

```shell
$ sudo apt install -y python3 python3-pip
```

<h2>安装NutstoreCLI</h2>

```shell
$ git clone https://github.com/Dreammer12138/NutstoreCLI.git
```

<h2>修改权限并添加到全局</h2>

```shell
$ sudo chmod a+x ./NutstoreCLI/Nutstore
$ sudo mv ./NutstoreCLI/Nutstore /usr/local/bin
```

# 用法

<h2>ls</h2>

```shell
$ Nutstore ls <remote_path>
```

打印远程路径中的文件目录。

- `remote_path`: 远程路径

<h2>mkdir</h2>

```shell
$ Nutstore mkdir <remote_path>
```

在远程路径中新建文件夹。

- `remote_path`: 远程路径

<h2>rm</h2>

```shell
$ Nutstore rm <remote_path>
```

删除远程路径中的文件或文件夹。

- `remote_path`: 远程路径

<h2>pull</h2>

```shell
$ Nutstore pull <remote_path> <local_path>
```

将文件或文件夹从远程路径下载到本地路径中。

- `remote_path`: 远程路径
- `local_path`: 本例路径

<h2>push</h2>

```shell
$ Nutstore push <remote_path> <local_path>
```

将文件或文件夹从本地路径推送到远程路径中。

- `remote_path`: 远程路径
- `local_path`: 本地路径

# 配置

```shell
$ Nutstore
Username: xxx@xxx.com
Password: 
```

第一次使用时将会要求您输入 `username` 和 `password` 。

配置文件将会被保存在 `~/.nutstore/config.json` 中。

你可以修改 `~/.nutstore/config.json` 文件去修改配置。

```json
{
    "username": "xxx@xxx.com",
    "password": "nutstore app key"
}
```

# Issues

如果您在使用中发现bug，请在本仓库下提交Issues，我将尽快解决。

如果您有更好的想法或者创意，可以自行 `clone` 代码，并将您的代码 `pull` 到本仓库中。

感谢您的使用。
