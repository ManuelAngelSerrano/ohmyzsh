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

  ```
      ZSH_THEME="simple"
  ```

- Añadir plugins en ~/.zshrc

  ```
      plugins=(git z sudo themes)
  ```

