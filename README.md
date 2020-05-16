# ohmyzsh
Mi configuración de ohmyzsh

- Instalar iTerm2 y configurar la tecla alt izquierda con ESC+
- Instalar zsh (si no está instalado)
- Instalar git, curl, wget
- Instalar ohmyzsh <https://ohmyz.sh/>
```shell 
    $ sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

- Cambiar el **tema** de zsh en ~/.zshrc <https://github.com/ohmyzsh/ohmyzsh/wiki/Themes>

```bash
    # Elegir entre simple, af-magic o agnoster
    # agnoster necesita una fuente parcheada powerline
    ZSH_THEME="simple"
    ZSH_THEME="af-magic"
    ZSH_THEME="agnoster"
    ZSH_THEME="powerlevel10k/powerlevel10k"
```
- Si quieres usar el tema **agnoster** o **PowerLevel10k**, instala las fuentes **Meslo_Nerd_Font** de <https://github.com/romkatv/powerlevel10k#meslo-nerd-font-patched-for-powerlevel10k> o **Meslo Dotted (Meslo LG L...)** de <https://github.com/powerline/fonts>  *(Añadidas la fuentes al repositorio)*
- Para usar **powerlevel10k** debes instalarlo antes <https://github.com/romkatv/powerlevel10k>
- Si usas **powerlevel10k** debes poner **"MesloLGS NF"** en **Visual Studio Code** como terminal font family

~~~shell
    git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/themes/powerlevel10k
~~~
- Añadir básicos **plugins** en ~/.zshrc <https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins>

_Info sobre atajos git en:_ <https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/git>
```bash
    # git para atajos de git 
    # z para saltar a los directorios más utilizados
    # sudo para poner sudo delante de la linea de comandos actual con <ESC><ESC>
    # themes para cambiar el tema sobre la marcha (theme y lsthemes)
    plugins=(git z sudo themes)
```

- Instalar:

**zsh-syntax-highlighting** <https://github.com/zsh-users/zsh-syntax-highlighting>

**Instalar zsh-autosuggestions** <https://github.com/zsh-users/zsh-autosuggestions>

```shell 
    git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
    git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```
**git-flow-avh** <https://github.com/petervanderdoes/gitflow-avh>

```shell 
brew install git-flow-avh
sudo apt-get install git-flow
yay gitflow-avh
```

- Añadir **plugins** en ~/.zshrc

```bash
    plugins=(git z sudo themes zsh-syntax-highlighting zsh-autosuggestions git-flow)
```

- Consultar el documento añadido sobre git-flow [gitglow-breakdown.pdf](https://github.com/ManuelAngelSerrano/ohmyzsh/blob/master/gitflow-breakdown.pdf) from <https://gist.github.com/ManuelAngelSerrano/fd4e3dd6b38e770afc39b1d3fc2225fd>

