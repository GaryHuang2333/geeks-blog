# iTerm2 + oh my zsh

## 1. iterm2
### 1.1 安装
[官网](https://iterm2.com/)直接下载安装

### 1.2 卸载


### 1.3 配置

---
---

## 2. oh my zsh
[官网介绍](https://github.com/ohmyzsh/ohmyzsh)  
- 思考: 这几种shell的区别 : /bin/bash, /bin/csh, /bin/dash, /bin/ksh, /bin/sh, /bin/tcsh, /bin/zsh

### 2.1 安装 
先确保本地安装了zsh, 并且版本新于5.0.8  
> 查看安装了的shell
> ```bash
> garyhuang@nuojiyaMBP14 ~ % cat /etc/shells 
> # List of acceptable shells for chpass(1).
> # Ftpd will not allow users to connect who are not using
> # one of these shells.
> 
> /bin/bash
> /bin/csh
> /bin/dash
> /bin/ksh
> /bin/sh
> /bin/tcsh
> /bin/zsh
> ```
> 
> 查看正在使用的shell
> ```bash
> garyhuang@nuojiyaMBP14 ~ % echo $SHELL
> /bin/zsh
> ```
>
> 查看zsh版本
> ```bash
> garyhuang@nuojiyaMBP14 ~ % zsh --version
> zsh --version
> zsh 5.8 (x86_64-apple-darwin21.0)
> ```
> 如果没安装, 可[参考安装zsh](https://github.com/ohmyzsh/ohmyzsh/wiki/Installing-ZSH)  
> 

然后根据[官网指令](https://ohmyz.sh/#install)安装 oh-my-zsh
```bash
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

不过国外源可能会有connection failure, 需要找国内源替换 

或者将***https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh***保存本地[./markdown_source/install.sh]运行, 
> 如果遇到[[SSL_ERROR_SYSCALL](https://www.cnblogs.com/life-of-coding/p/12822614.html)], 要将ipv6禁用，“系统偏好设置”->"网络"->选择对应的网卡->"高级"->"配置ipv6",选择适合自己的选项，本人选择的是仅本地连接。记得点击"应用"  

### 2.2 卸载
- If you want to uninstall oh-my-zsh, just run ```uninstall_oh_my_zsh``` from the command-line. It will remove itself and revert your previous bash or zsh configuration.  

- 只需在命令行运行 ```uninstall_oh_my_zsh``` 就可以简单卸载oh-my-zsh 并恢复回原有的bash或zsh配置  

- [参考链接](https://github.com/ohmyzsh/ohmyzsh#uninstalling-oh-my-zsh)

### 2.3 配置
1. oh-my-zsh 默认安装在 **~/.oh-my-zsh**  
2. MacOS 没有自带 **~/.zshrc** 文件, 如果安装 oh-my-zsh 后发现也没有, 需要自己新建一个来配置oh-my-zsh


- 如何使用插件(https://github.com/ohmyzsh/ohmyzsh#plugins)
- 如何更换主题(https://github.com/ohmyzsh/ohmyzsh#themes)




