# Flatpak

## 安装 Flatpak {id="flatpak_1"}

```bash
sudo apt install flatpak 
```

## 配置 Flatpak 仓库地址

```bash
flatpak remote-add --if-not-exists flathub https://dl.flathub.org/repo/flathub.flatpakrepo
```

## 配置环境变量

如果使用 **Bash**, 则修改 **.bashrc** 文件

```bash
echo 'export XDG_DATA_DIRS=$XDG_DATA_DIRS:/var/lib/flatpak/exports/share:$HOME/.local/share/flatpak/exports/share' >> ~/.bashrc
```

如果使用 **Zsh**, 则修改 **.zshrc** 文件

```
echo 'export XDG_DATA_DIRS=$XDG_DATA_DIRS:/var/lib/flatpak/exports/share:$HOME/.local/share/flatpak/exports/share' >> ~/.zshrc
```

## 重启

以上安装、配置需要重启生效