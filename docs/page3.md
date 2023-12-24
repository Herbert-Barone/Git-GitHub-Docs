
# **Instalando o Git**

## Windows & macOS

Para ambos sistemas deve-se baixar o instalador no site official do [Git](page2.md\#o-que-e-o-git).

- Página oficial de download para [Windows](https://git-scm.com/download/win).
- Página oficial de download para [macOS](https://git-scm.com/download/mac).


## Distribuições Linux

Veja abaixo como **instalar** o [Git](page2.md\#o-que-e-o-git) em **algumas** das principais **distribuições** do **Linux**.

!!! Nota 
    Caso necessite de privilégios de administrador utilize o comando **sudo** antes dos códigos:
    
    > Exemplo:
        ```
        sudo apt-get install git 
        ```

- Página oficial referente a documentação de instalação do [Git](page2.md\#o-que-e-o-git) nas [Distribuições Linux](https://git-scm.com/download/linux).


### Debian/Ubuntu

```
apt-get install git 
```

### Ubuntu

```
add-apt-repository ppa:git-core/ppa     # Primeiro Comando.
```
```
apt update                              # Segundo Comando.
```
```
apt install git                         # Terceiro Comando.
```

### Fedora

```
yum install git                         # Até o Fedora 21.
```
```
dnf install git                         # Fedora 22 e os próximos.
```

### Arch Linux

```
pacman -S git                           # Único Comando.
```

### Alpine
```
$ apk add git                           # Único Comando.
```
