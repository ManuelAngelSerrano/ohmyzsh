# ohmyzsh
Mi configuración de ohmyzsh

- Instalar iTerm2 y configurar la tecla alt izquierda con ESC+
- Instalar zsh (si no está instalado)
- Instalar git, curl, wget
- Instalar ohmyzsh <https://ohmyz.sh/>
```shell 
    $ sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

- Cambiar el tema de zsh en ~/.zshrc

```bash
    ZSH_THEME="simple"
```

- Añadir plugins en ~/.zshrc

```bash
    plugins=(git z sudo themes)
```

- Instalar zsh-syntax-highlighting <https://github.com/zsh-users/zsh-syntax-highlighting>

```shell 
    git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```
- Añadir plugins en ~/.zshrc

```bash
    plugins=(git z sudo themes zsh-syntax-highlighting)
```

- Instalar zsh-autosuggestions <https://github.com/zsh-users/zsh-autosuggestions>

```shell 
    git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```


- Añadir plugins en ~/.zshrc

```bash
    plugins=(git z zsh-autosuggestions sudo themes zsh-syntax-highlighting)
```
