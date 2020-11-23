<h1>Nutstore CLI</h1>

[![PYVERSION](https://img.shields.io/badge/Python-3.7.3-blue)](https://www.python.org) [![CURL](https://img.shields.io/badge/cURL-green)](http://curl.haxx.se)

Nutstore command line tool in Linux.

# Install

## Install python3.7 and later version

Take Debian as an example

```shell
$ sudo apt install -y python3 python3-pip
```

## Install NutstoreCLI

```shell
$ git clone https://github.com/Dreammer12138/NutstoreCLI.git
```

## Modify permissions and add to global

```shell
$ sudo chmod a+x ./NutstoreCLI/Nutstore
$ sudo mv ./NutstoreCLI/Nutstore /usr/local/bin
```

# Usage

## ls

```shell
$ Nutstore ls <remote_path>
```

Print out the file directory in remote path.

- `remote_path`: Remote path in nutstore

## mkdir

```shell
$ Nutstore mkdir <remote_path>
```

Create directory in remote path.

- `remote_path`: Remote path in nutstore

## rm

```shell
$ Nutstore rm <remote_path>
```

Remove directory or file in remote path.

- `remote_path`: Remote path in nutstore

## pull

```shell
$ Nutstore pull <remote_path> <local_path>
```

Pull directory and file to local path from remote path.

- `remote_path`: Remote path in nutstore
- `local_path`: Local path

## push

```shell
$ Nutstore push <remote_path> <local_path>
```

Push directory and file to remote path from local path.

- `remote_path`: Remote path in nutstore
- `local_path`: Local path

# Config

```shell
$ Nutstore
Username: xxx@xxx.com
Password: 
```

Input username and password will be required the first time you use it.

Configuration information will be saved in the `~/.nutstore/config.json` .

You can change `~/.nutstore/config.json` to configure user information.

```json
{
    "username": "xxx@xxx.com",
    "password": "nutstore app key"
}
```

# Issus

If you find bug in use, please submit Issus in this repository and I will solve it as soon as possible.

If you have better ideas, you can clone by yourself and pull your code to the repository.

Thanks for using.

>  <small>Translate by 腾讯翻译君</small>